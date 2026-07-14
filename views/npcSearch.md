```dataviewjs
/**********************************************************************
 * NPC SEARCH VIEW
 *
 * Parte 1/3
 *
 * Costruzione GUI
 * - scansione ruoli
 * - widget
 * - layout
 **********************************************************************/

// --------------------------------------------------
// CONFIG
// --------------------------------------------------

const NPC_ROOT = '"NPCs"';

// --------------------------------------------------
// ROOT CONTAINER
// --------------------------------------------------

const root = dv.container;

root.innerHTML = "";

const wrapper = root.createDiv({
    cls: "npc-search"
});

wrapper.style.display = "flex";
wrapper.style.flexDirection = "column";
wrapper.style.rowGap = "1em";


// --------------------------------------------------
// TITLE
// --------------------------------------------------

wrapper.createEl("h2", {
    text: "NPC Search"
});


// --------------------------------------------------
// FILTER PANEL
// --------------------------------------------------

const filterPanel = wrapper.createDiv();

filterPanel.style.display = "flex";
filterPanel.style.flexWrap = "wrap";
filterPanel.style.gap = "1em";
filterPanel.style.alignItems = "flex-end";


// --------------------------------------------------
// RESULT PANEL
// --------------------------------------------------

const resultPanel = wrapper.createDiv();


// --------------------------------------------------
// HELPERS
// --------------------------------------------------

function makeField(labelText)
{
    const field = filterPanel.createDiv();

    field.style.display = "flex";
    field.style.flexDirection = "column";
    field.style.minWidth = "180px";

    field.createEl("label", {
        text: labelText
    });

    return field;
}


function makeSelect(field)
{
    const select = field.createEl("select");

    select.style.width = "100%";

    return select;
}


function makeNumber(field, value = 0)
{
    const input = field.createEl("input");

    input.type = "number";
    input.value = value;

    input.style.width = "80px";

    return input;
}


// --------------------------------------------------
// CONTROLS
// --------------------------------------------------

const roleField = makeField("Role");
const roleSelect = makeSelect(roleField);

const operatorField = makeField("Operator");
const operatorSelect = makeSelect(operatorField);

const rankField = makeField("Minimum rank");
const rankInput = makeNumber(rankField, 0);


// --------------------------------------------------
// OPERATOR LIST
// --------------------------------------------------

[
    "=",
    ">",
    ">=",
    "<",
    "<="
].forEach(op =>
{
    const option = document.createElement("option");

    option.value = op;
    option.textContent = op;

    operatorSelect.appendChild(option);
});

operatorSelect.value = ">=";


// --------------------------------------------------
// PRE-SCAN NPCs
// --------------------------------------------------

const npcPages = dv
    .pages(NPC_ROOT)
    .where(p => p.role);


// --------------------------------------------------
// EXTRACT ALL ROLES
// --------------------------------------------------

const roles = new Set();

for (const npc of npcPages)
{
    if (!Array.isArray(npc.role))
        continue;

    for (const role of npc.role)
    {
        if (!role)
            continue;

        roles.add(String(role));
    }
}

const sortedRoles =
    Array.from(roles)
         .sort((a, b) => a.localeCompare(b));


// --------------------------------------------------
// POPULATE ROLE SELECT
// --------------------------------------------------

{
    const any = document.createElement("option");

    any.value = "";

    any.textContent = "Any";

    roleSelect.appendChild(any);

    for (const role of sortedRoles)
    {
        const option = document.createElement("option");

        option.value = role;
        option.textContent = role;

        roleSelect.appendChild(option);
    }
}


// --------------------------------------------------
// COMPARISON
// --------------------------------------------------

function compare(left, operator, right)
{
    switch (operator)
    {
        case "=":
            return left === right;

        case ">":
            return left > right;

        case ">=":
            return left >= right;

        case "<":
            return left < right;

        case "<=":
            return left <= right;

        default:
            return false;
    }
}


// --------------------------------------------------
// NPC MATCH
// --------------------------------------------------

function npcMatches(npc)
{
    const selectedRole = roleSelect.value;
    const operator = operatorSelect.value;
    const wantedRank = Number(rankInput.value);

    if (!npc.role || !npc.rank)
        return false;

    if (!Array.isArray(npc.role))
        return false;

    if (!Array.isArray(npc.rank))
        return false;

    if (npc.role.length !== npc.rank.length)
        return false;

    // --------------------------------------------------
    // Any role
    // --------------------------------------------------

    if (selectedRole === "")
    {
        for (let i = 0; i < npc.rank.length; i++)
        {
            const rank = Number(npc.rank[i]);

            if (compare(rank, operator, wantedRank))
                return true;
        }

        return false;
    }

    // --------------------------------------------------
    // Specific role
    // --------------------------------------------------

    for (let i = 0; i < npc.role.length; i++)
    {
        const role = String(npc.role[i]);

        if (role !== selectedRole)
            continue;

        const rank = Number(npc.rank[i]);

        if (compare(rank, operator, wantedRank))
            return true;
    }

    return false;
}


// --------------------------------------------------
// BUILD RESULT LIST
// --------------------------------------------------

function computeResults()
{
    const result = [];

    for (const npc of npcPages)
    {
        if (!npcMatches(npc))
            continue;

        result.push(npc);
    }

    result.sort((a, b) =>
        a.file.name.localeCompare(b.file.name)
    );

    return result;
}


// --------------------------------------------------
// RENDER ENTRY
// --------------------------------------------------

function buildRoleString(npc)
{
    const parts = [];

    for (let i = 0; i < npc.role.length; i++)
    {
        parts.push(
            `${npc.role[i]} (${npc.rank[i]})`
        );
    }

    return parts.join(", ");
}


// --------------------------------------------------
// REFRESH
// --------------------------------------------------

function refresh()
{
    const results = computeResults();

    resultPanel.innerHTML = "";

    resultPanel.createEl("p", {
        text: `${results.length} NPC found`
    });

    renderTable(results);
}


// --------------------------------------------------
// INITIAL RENDER
// --------------------------------------------------

refresh();


// --------------------------------------------------
// EVENTS
// --------------------------------------------------

roleSelect.onchange = refresh;

operatorSelect.onchange = refresh;

rankInput.oninput = refresh;

// --------------------------------------------------
// TABLE RENDERING
// --------------------------------------------------

function getFolder(page)
{
    const parts = page.file.path.split("/");

    // Rimuove il nome del file
    parts.pop();

    // Rimuove "NPCs"
    if (parts.length && parts[0] === "NPCs")
        parts.shift();

    return parts.join(" / ");
}

function renderTable(results)
{
    const table = resultPanel.createEl("table");

    table.style.width = "100%";
    table.style.borderCollapse = "collapse";

    //--------------------------------------------------
    // HEADER
    //--------------------------------------------------

    const thead = table.createEl("thead");
    const headRow = thead.createEl("tr");

    [
        "NPC",
        "Roles",
        "Folder"
    ].forEach(text =>
    {
        const th = headRow.createEl("th", {
            text
        });

        th.style.textAlign = "left";
        th.style.padding = "6px";
        th.style.borderBottom = "1px solid var(--background-modifier-border)";
    });

    //--------------------------------------------------
    // BODY
    //--------------------------------------------------

    const tbody = table.createEl("tbody");

    for (const npc of results)
    {
        const row = tbody.createEl("tr");

        //----------------------------------------------
        // NPC
        //----------------------------------------------

		const npcCell = row.createEl("td");
		
		npcCell.style.padding = "6px";
		
		const link = npcCell.createEl("a", {
		    text: npc.file.name,
		    href: npc.file.path
		});
		
		link.addClass("internal-link");
		link.dataset.href = npc.file.path;

        //----------------------------------------------
        // Roles
        //----------------------------------------------

        const roleCell = row.createEl("td", {
            text: buildRoleString(npc)
        });

        roleCell.style.padding = "6px";

        //----------------------------------------------
        // Folder
        //----------------------------------------------

        const folderCell = row.createEl("td", {
            text: getFolder(npc)
        });

        folderCell.style.padding = "6px";
    }

    //--------------------------------------------------
    // Empty state
    //--------------------------------------------------

    if (results.length === 0)
    {
        const p = resultPanel.createEl("p", {
            text: "No NPC matches the current filters."
        });

        p.style.opacity = "0.7";
    }
}

```