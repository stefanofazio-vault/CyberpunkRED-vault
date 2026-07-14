```dataviewjs
/**********************************************************************
 * npcSearch.js
 *
 * Parte 1/3
 *
 * - Configurazione
 * - Utility DOM
 * - Renderer
 * - Classe Table
 **********************************************************************/

// ======================================================
// CONFIGURATION
// ======================================================

const NPC_ROOT = '"NPCs"';

// ======================================================
// ROOT
// ======================================================

const root = dv.container;

root.empty();

const appContainer = root.createDiv({
    cls: "npc-search"
});

appContainer.style.display = "flex";
appContainer.style.flexDirection = "column";
appContainer.style.gap = "1rem";

// ======================================================
// TITLE
// ======================================================

appContainer.createEl("h2", {
    text: "NPC Search"
});

// ======================================================
// FILTER PANEL
// ======================================================

const filterPanel = appContainer.createDiv();

filterPanel.style.display = "flex";
filterPanel.style.flexWrap = "wrap";
filterPanel.style.alignItems = "end";
filterPanel.style.gap = "1rem";

// ======================================================
// RESULT PANEL
// ======================================================

const resultPanel = appContainer.createDiv();

// ======================================================
// DOM HELPERS
// ======================================================

function createField(label)
{
    const field = filterPanel.createDiv();

    field.style.display = "flex";
    field.style.flexDirection = "column";
    field.style.gap = "4px";
    field.style.minWidth = "180px";

    field.createEl("label", {
        text: label
    });

    return field;
}

function createSelect(parent)
{
    const select = parent.createEl("select");

    select.style.width = "100%";

    return select;
}

function createNumber(parent, value = 0)
{
    const input = parent.createEl("input");

    input.type = "number";
    input.value = value;

    input.style.width = "90px";

    return input;
}

function addOption(select, text, value = text)
{
    const option = document.createElement("option");

    option.textContent = text;
    option.value = value;

    select.appendChild(option);
}

// ======================================================
// GENERIC HELPERS
// ======================================================

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

function getFolder(page)
{
    const path = page.file.path.split("/");

    path.pop();

    if (path[0] === "NPCs")
        path.shift();

    return path.join(" / ");
}

function getLinkLabel(value)
{
    if (value == null)
        return "";

    // Link Dataview
    if (typeof value === "object" && value.path)
    {
        return value.display ??
            value.path
                .split("/")
                .pop()
                .replace(/\.md$/, "");
    }

    // Stringa semplice
    let text = String(value);

    // Wikilink?
    const match = text.match(/^\[\[(.+?)\]\]$/);

    if (match)
    {
        text = match[1];
    }

    // Alias?
    if (text.includes("|"))
    {
        text = text.split("|").pop();
    }

    // Percorso?
    if (text.includes("/"))
    {
        text = text.split("/").pop();
    }

    return text.replace(/\.md$/, "");
}

// ======================================================
// WIKILINK RENDERER
// ======================================================

function renderWikiLink(parent, page)
{
    const link = parent.createEl("a", {
        text: page.file.name,
        href: page.file.path
    });

    link.addClass("internal-link");
    link.dataset.href = page.file.path;
}

// ======================================================
// ROLE RENDERER
// ======================================================

function renderRoles(parent, npc)
{
    if (!npc.role || !npc.rank)
        return;

    for (let i = 0; i < npc.role.length; i++)
    {
        const line = parent.createDiv();

        line.style.display = "flex";
        line.style.justifyContent = "space-between";
        line.style.gap = "1rem";

        line.createSpan({
            text: String(npc.role[i])
        });

        const rank = line.createSpan({
            text: String(npc.rank[i])
        });

        rank.style.opacity = "0.75";
        rank.style.fontWeight = "600";
    }
}

function renderInternalLink(parent, link)
{
    const a = parent.createEl("a", {
        text: getLinkLabel(link),
        href: link.path
    });

    a.addClass("internal-link");
    a.dataset.href = link.path;
}

function renderAffiliations(parent, npc)
{
    if (!npc.affiliation)
        return;

    const affiliations = Array.isArray(npc.affiliation)
        ? npc.affiliation
        : [npc.affiliation];

    for (const affiliation of affiliations)
    {
        const line = parent.createDiv();

		if (typeof affiliation === "object")
		{
		    renderInternalLink(line, affiliation);
		}
		else
		{
		    line.setText(getLinkLabel(affiliation));
		}
    }
}

// ======================================================
// TABLE COMPONENT
// ======================================================

class Table
{
    constructor(parent)
    {
        this.parent = parent;
        this.columns = [];
    }

    addColumn(title, renderer)
    {
        this.columns.push({
            title,
            renderer
        });
    }

    render(rows)
    {
        this.parent.empty();

        const table = this.parent.createEl("table");

        table.style.width = "100%";
        table.style.borderCollapse = "collapse";

        //--------------------------------------------------

        const thead = table.createEl("thead");

        const head = thead.createEl("tr");

        for (const column of this.columns)
        {
            const th = head.createEl("th");

            th.setText(column.title);

            th.style.textAlign = "left";
            th.style.padding = "6px";
            th.style.borderBottom =
                "1px solid var(--background-modifier-border)";
        }

        //--------------------------------------------------

        const tbody = table.createEl("tbody");

        for (const row of rows)
        {
            const tr = tbody.createEl("tr");

            for (const column of this.columns)
            {
                const td = tr.createEl("td");

                td.style.padding = "6px";
                td.style.verticalAlign = "top";

                column.renderer(td, row);
            }
        }

        //--------------------------------------------------

        if (rows.length === 0)
        {
            const p = this.parent.createEl("p", {
                text: "No NPC matches the current filters."
            });

            p.style.opacity = "0.7";
        }
    }
}

// ======================================================
// TABLE INSTANCE
// ======================================================

const table = new Table(resultPanel);

// ======================================================
// NPC CACHE
// ======================================================

const npcPages = dv
    .pages(NPC_ROOT)
    .where(p => p.file);

// ======================================================
// EXTRACT AVAILABLE ROLES
// ======================================================

const availableRoles = new Set();

for (const npc of npcPages)
{
    if (!npc.role)
        continue;

    const roles = Array.isArray(npc.role)
        ? npc.role
        : [npc.role];

    for (const role of roles)
    {
        if (role == null)
            continue;

        availableRoles.add(String(role));
    }
}

const sortedRoles =
    [...availableRoles]
        .sort((a, b) => a.localeCompare(b));

// ======================================================
// EXTRACT AVAILABLE AFFILIATIONS
// ======================================================

const availableAffiliations = new Set();

for (const npc of npcPages)
{
    if (!npc.affiliation)
        continue;

    const affiliations = Array.isArray(npc.affiliation)
        ? npc.affiliation
        : [npc.affiliation];

    for (const affiliation of affiliations)
    {
		availableAffiliations.add(getLinkLabel(affiliation));
    }
}

const sortedAffiliations =
    [...availableAffiliations]
        .sort((a, b) => a.localeCompare(b));

// ======================================================
// FILTERS
// ======================================================

const filters = {};

//
// Role
//

{
    const field = createField("Role");

    filters.role = createSelect(field);

    addOption(filters.role, "Any", "");

    for (const role of sortedRoles)
        addOption(filters.role, role);
}

//
// Operator
//

{
    const field = createField("Rank");

    filters.operator = createSelect(field);

    [
        "=",
        ">",
        ">=",
        "<",
        "<="
    ].forEach(op =>
    {
        addOption(filters.operator, op);
    });

    filters.operator.value = ">=";
}

//
// Rank
//

{
    const field = createField("Minimum Rank");

    filters.rank = createNumber(field, 0);

    filters.rank.min = 0;
}

//
// Affiliation
//

{
	const field = createField("Affiliation");
	
	filters.affiliation = createSelect(field);
	
	addOption(filters.affiliation, "Any", "");
	
	for (const affiliation of sortedAffiliations)
	{
	    addOption(filters.affiliation, affiliation);
	}

}

// ======================================================
// FILTER STATE
// ======================================================

filters.values = function ()
{
    return {

        role: this.role.value,

        operator: this.operator.value,

        rank: Number(this.rank.value),
        
        affiliation: this.affiliation.value

    };
};

// ======================================================
// MATCHING
// ======================================================

function npcMatches(npc)
{
    const f = filters.values();
    
    if ((f.affiliation === "" || f.affiliation === "Any") && 
		f.role === "" && f.rank === 0)
		return true;
    
    var affiliationFound = false;

    const roles =
        Array.isArray(npc.role)
            ? npc.role
            : [npc.role];

    const ranks =
        Array.isArray(npc.rank)
            ? npc.rank
            : [npc.rank];
            
	const affiliations =
		(Array.isArray(npc.affiliation)
			? npc.affiliation
			: [npc.affiliation]);
		

    //--------------------------------------------------
    // Parallel arrays must match
    //--------------------------------------------------

    if (roles.length !== ranks.length)
        return false;

	if (f.affiliation !== "" && f.affiliation !== "Any")
	{
	    affiliationFound = false;
	
	    for (const affiliation of affiliations)
	    {
			if (getLinkLabel(affiliation) === f.affiliation)
			{
			    affiliationFound = true;
			    break;
			}
	    }
	
	    if (!affiliationFound)
	        return false;
	}
	
    //--------------------------------------------------
    // Iterate every role
    //--------------------------------------------------
    if (f.role !== "" || f.rank > 0)
    {
	    for (let i = 0; i < roles.length; i++)
	    {
	        const role = String(roles[i]);
	
	        const rank = Number(ranks[i]);
	
	        //--------------------------------------------------
	        // Any role selected
	        //--------------------------------------------------
	
	        if (f.role === "")
	        {
	            if (compare(rank, f.operator, f.rank))
	                return true;
	
	            continue;
	        }
	
	        //--------------------------------------------------
	        // Specific role
	        //--------------------------------------------------
	
	        if (role !== f.role)
	            continue;
	
	        if (compare(rank, f.operator, f.rank))
	            return true;
	    }
	}
	else
	{
		return affiliationFound;
    }

    return false;
}

// ======================================================
// FILTER EVENTS
// ======================================================

filters.role.onchange = refresh;

filters.operator.onchange = refresh;

filters.rank.oninput = refresh;

filters.affiliation.oninput = refresh;

// ======================================================
// COMPUTE RESULTS
// ======================================================

function computeResults()
{
    const results = [];

    for (const npc of npcPages)
    {
        if (npcMatches(npc))
            results.push(npc);
    }

    results.sort((a, b) =>
        a.file.name.localeCompare(
            b.file.name,
            undefined,
            { sensitivity: "base" }
        )
    );

    return results;
}

// ======================================================
// TABLE DEFINITION
// ======================================================

table.addColumn(
    "NPC",
    (cell, npc) =>
    {
        renderWikiLink(cell, npc);
    }
);

table.addColumn(
    "Roles",
    (cell, npc) =>
    {
        renderRoles(cell, npc);
    }
);

table.addColumn(
	"Affiliations",
	(cell, npc) =>
	{
		renderAffiliations(cell, npc);
	}
);

table.addColumn(
    "Folder",
    (cell, npc) =>
    {
        cell.setText(getFolder(npc));
    }
);

// ======================================================
// REFRESH
// ======================================================

function refresh()
{
    const results = computeResults();

    resultPanel.empty();

    resultPanel.createEl("div", {
        text: `${results.length} NPC found`
    });

    table.parent = resultPanel;

    table.render(results);
}

// ======================================================
// INITIAL RENDER
// ======================================================

refresh();
```
