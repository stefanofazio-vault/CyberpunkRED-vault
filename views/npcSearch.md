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
    if (!link)
        return;

    let path;
    let label;

    if (typeof link === "object")
    {
        path = link.path;
        label = getLinkLabel(link);
    }
    else
    {
        path = String(link);
        label = getLinkLabel(link);
    }

    const a = parent.createEl("a", {
        text: label,
        href: path
    });

    a.addClass("internal-link");
    a.dataset.href = path;
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

function renderDistrict(parent, npc)
{
    if (!npc.location)
        return;

    const locations =
        Array.isArray(npc.location)
            ? npc.location
            : [npc.location];

    const rendered = new Set();

    for (const location of locations)
    {
        if (!location)
            continue;

        let path = null;

        if (typeof location === "object" && location.path)
        {
            path = location.path;
        }
        else
        {
            const match =
                String(location)
                    .match(/^\[\[(.+?)(\|.+?)?\]\]$/);

            if (match)
                path = match[1];
        }

        if (!path)
            continue;

        const district = districtCache.get(path);

        if (!district)
            continue;

        if (rendered.has(district.label))
            continue;

        rendered.add(district.label);

        const line = parent.createDiv();

        renderInternalLink(line, district.link);
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
// DISTRICT CACHE
// ======================================================

const neighbourhoodPages =
    dv.pages('"Neighbourhoods"')
      .where(p => p.file);

const locationPages =
    dv.pages('"Locations"')
      .where(p => p.file);

// path -> page
const locationMap = new Map();

for (const page of locationPages)
{
    locationMap.set(page.file.path, page);
}

// path -> district page
const districtCache = new Map();

function getLocationTarget(page)
{
    if (!page.location)
        return null;

    const value =
        Array.isArray(page.location)
            ? page.location[0]
            : page.location;

    if (!value)
        return null;

    if (typeof value === "object")
        return value;

    return null;
}

function resolveDistrict(page)
{
    if (!page)
        return null;

    //--------------------------------------------------
    // depth 0
    //--------------------------------------------------

    let target = getLocationTarget(page);

    if (!target)
        return null;

    if (target.path.startsWith("Neighbourhoods/"))
        return target;

    //--------------------------------------------------
    // depth 1
    //--------------------------------------------------

    let page1 = locationMap.get(target.path);

    if (!page1)
        return null;

    target = getLocationTarget(page1);

    if (!target)
        return null;

    if (target.path.startsWith("Neighbourhoods/"))
        return target;

    //--------------------------------------------------
    // depth 2
    //--------------------------------------------------

    let page2 = locationMap.get(target.path);

    if (!page2)
        return null;

    target = getLocationTarget(page2);

    if (!target)
        return null;

    if (target.path.startsWith("Neighbourhoods/"))
        return target;

    return null;
}

//------------------------------------------------------
// Build cache
//------------------------------------------------------

for (const page of neighbourhoodPages)
{
	districtCache.set(
	    page.file.path,
	    {
	        label: page.file.name,
	        link: page.file.link,
	        path: page.file.path
	    }
	);
}

for (const page of locationPages)
{
    const district = resolveDistrict(page);

    if (!district)
        continue;

	districtCache.set(
	    page.file.path,
	    {
	        label: getLinkLabel(district),
	        link: district,
	        path: district.path
	    }
	);
}

// ======================================================
// AVAILABLE DISTRICTS
// ======================================================

const availableDistricts =
    [...neighbourhoodPages]
        .map(p => p.file.name)
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

//
// District
//

{
    const field = createField("District");

    filters.district = createSelect(field);

    addOption(filters.district, "Any", "");

    for (const district of availableDistricts)
    {
        addOption(filters.district, district);
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
        
        affiliation: this.affiliation.value,
        
        district: this.district.value

    };
};

// ======================================================
// DISTRICT MATCHING
// ======================================================

function npcInDistrict(npc, districtName)
{
    if (!npc.location)
        return false;

    const locations =
        Array.isArray(npc.location)
            ? npc.location
            : [npc.location];

    for (const location of locations)
    {
        if (!location)
            continue;

        //--------------------------------------------------
        // Dataview Link
        //--------------------------------------------------

        if (typeof location === "object" && location.path)
        {
            const district = districtCache.get(location.path);

            if (!district)
                continue;

            if (district.label === districtName)
                return true;

            continue;
        }

        //--------------------------------------------------
        // String wikilink
        //--------------------------------------------------

        const text = String(location);

        const match =
            text.match(/^\[\[(.+?)(\|.+?)?\]\]$/);

        if (!match)
            continue;

        const path = match[1];

        const district = districtCache.get(path);

        if (!district)
            continue;

        if (district.label === districtName)
            return true;
    }

    return false;
}

// ======================================================
// MATCHING
// ======================================================

function npcMatches(npc)
{
    const f = filters.values();

    //--------------------------------------------------
    // No filters
    //--------------------------------------------------

    if (
        (f.affiliation === "" || f.affiliation === "Any") &&
        (f.district === "" || f.district === "Any") &&
        f.role === "" &&
        f.rank === 0
    )
    {
        return true;
    }

    //--------------------------------------------------
    // Roles / Ranks
    //--------------------------------------------------

    const roles =
        Array.isArray(npc.role)
            ? npc.role
            : (npc.role ? [npc.role] : []);

    const ranks =
        Array.isArray(npc.rank)
            ? npc.rank
            : (npc.rank ? [npc.rank] : []);

    if (roles.length !== ranks.length)
        return false;

    //--------------------------------------------------
    // Affiliation
    //--------------------------------------------------

    if (f.affiliation !== "" && f.affiliation !== "Any")
    {
        const affiliations =
            Array.isArray(npc.affiliation)
                ? npc.affiliation
                : (npc.affiliation ? [npc.affiliation] : []);

        let found = false;

        for (const affiliation of affiliations)
        {
            if (getLinkLabel(affiliation) === f.affiliation)
            {
                found = true;
                break;
            }
        }

        if (!found)
            return false;
    }

    //--------------------------------------------------
    // District
    //--------------------------------------------------

    if (f.district !== "" && f.district !== "Any")
    {
        if (!npcInDistrict(npc, f.district))
            return false;
    }

    //--------------------------------------------------
    // Role disabled
    //--------------------------------------------------

    if (f.role === "" && f.rank === 0)
        return true;

    //--------------------------------------------------
    // Role matching
    //--------------------------------------------------

    for (let i = 0; i < roles.length; i++)
    {
        const role = String(roles[i]);
        const rank = Number(ranks[i]);

        if (f.role === "")
        {
            if (compare(rank, f.operator, f.rank))
                return true;

            continue;
        }

        if (role !== f.role)
            continue;

        if (compare(rank, f.operator, f.rank))
            return true;
    }

    return false;
}

// ======================================================
// FILTER EVENTS
// ======================================================

filters.role.onchange = refresh;

filters.operator.onchange = refresh;

filters.rank.oninput = refresh;

filters.affiliation.onchange = refresh;

filters.district.onchange = refresh;

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
    "District",
    (cell, npc) =>
    {
        renderDistrict(cell, npc);
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
