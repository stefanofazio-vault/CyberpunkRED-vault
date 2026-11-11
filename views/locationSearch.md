```dataviewjs

// ======================================================

// CONFIGURATION

// ======================================================

const LOCATION_ROOT = '"Locations"';

// ======================================================

// ROOT

// ======================================================

const root = dv.container;

root.empty();

const appContainer = root.createDiv({

    cls: "location-search"

});

appContainer.style.display = "flex";

appContainer.style.flexDirection = "column";

appContainer.style.gap = "1rem";

// ======================================================

// TITLE

// ======================================================

appContainer.createEl("h2", {

    text: "Location Search"

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

    field.createEl("label", { text: label });

    return field;

}

function createSelect(parent)

{

    const select = parent.createEl("select");

    select.style.width = "100%";

    return select;

}

function addOption(select, text, value = text)

{

    const option = document.createElement("option");

    option.textContent = text;

    option.value = value;

    select.appendChild(option);

}

// ======================================================

// HELPERS

// ======================================================

function getLinkLabel(value)

{

    if (value == null)

        return "";

    if (typeof value === "object" && value.path)

    {

        return value.display ??

            value.path

                .split("/")

                .pop()

                .replace(/\.md$/, "");

    }

    let text = String(value);

    const wiki =

        text.match(/^\[\[(.+?)\]\]$/);

    if (wiki)

    {

        text = wiki[1];

    }

    if (text.includes("|"))

    {

        text = text.split("|").pop();

    }

    if (text.includes("/"))

    {

        text = text.split("/").pop();

    }

    return text.replace(/\.md$/, "");

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

function renderWikiLink(parent, page)

{

    const link = parent.createEl("a", {

        text: page.file.name,

        href: page.file.path

    });

    link.addClass("internal-link");

    link.dataset.href = page.file.path;

}

function getLocationType(page)

{

    const parts = page.file.path.split("/");

    if (parts.length < 3)

        return "";

    return parts[1];

}

// ======================================================

// RENDERERS

// ======================================================

function renderDistrict(cell, location)

{

    if (!location.location)

        return;

    const districts =

        Array.isArray(location.location)

            ? location.location

            : [location.location];

    for (const district of districts)

    {

        const row = cell.createDiv();

        if (typeof district === "object")

        {

            renderInternalLink(row, district);

        }

        else

        {

            row.setText(getLinkLabel(district));

        }

    }

}

function renderAffiliations(cell, location)

{

    if (!location.affiliation)

        return;

    const affiliations =

        Array.isArray(location.affiliation)

            ? location.affiliation

            : [location.affiliation];

    for (const affiliation of affiliations)

    {

        const row = cell.createDiv();

        if (typeof affiliation === "object")

        {

            renderInternalLink(row, affiliation);

        }

        else

        {

            row.setText(getLinkLabel(affiliation));

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

        if (rows.length === 0)

        {

            const p = this.parent.createEl("p", {

                text: "No location matches the current filters."

            });

            p.style.opacity = "0.7";

        }

    }

}

// ======================================================

// TABLE

// ======================================================

const table = new Table(resultPanel);

// ======================================================

// LOCATION CACHE

// ======================================================

const locationPages =

    dv.pages(LOCATION_ROOT)

      .where(p => p.file);

// ======================================================

// AVAILABLE TYPES

// ======================================================

const availableTypes = new Set();

for (const page of locationPages)

{

    const type = getLocationType(page);

    if (type)

    {

        availableTypes.add(type);

    }

}

const sortedTypes =

    [...availableTypes]

        .sort((a, b) =>

            a.localeCompare(b));

// ======================================================

// AVAILABLE DISTRICTS

// ======================================================

const availableDistricts = new Set();

for (const page of locationPages)

{

    const districts =

        Array.isArray(page.location)

            ? page.location

            : (page.location ? [page.location] : []);

    for (const district of districts)

    {

        availableDistricts.add(

            getLinkLabel(district)

        );

    }

}

const sortedDistricts =

    [...availableDistricts]

        .sort((a, b) =>

            a.localeCompare(b));

// ======================================================

// AVAILABLE AFFILIATIONS

// ======================================================

const availableAffiliations = new Set();

for (const page of locationPages)

{

    if (!page.affiliation)

        continue;

    const affiliations =

        Array.isArray(page.affiliation)

            ? page.affiliation

            : [page.affiliation];

    for (const affiliation of affiliations)

    {

        availableAffiliations.add(

            getLinkLabel(affiliation)

        );

    }

}

const sortedAffiliations =

    [...availableAffiliations]

        .sort((a, b) =>

            a.localeCompare(b));

// ======================================================

// FILTERS

// ======================================================

const filters = {};

// Type

{

    const field = createField("Type");

    filters.type = createSelect(field);

    addOption(filters.type, "Any", "");

    for (const type of sortedTypes)

    {

        addOption(filters.type, type);

    }

}

// District

{

    const field = createField("District");

    filters.district = createSelect(field);

    addOption(filters.district, "Any", "");

    for (const district of sortedDistricts)

    {

        addOption(filters.district, district);

    }

}

// Affiliation

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

// FILTER VALUES

// ======================================================

filters.values = function ()

{

    return {

        type: this.type.value,

        district: this.district.value,

        affiliation: this.affiliation.value

    };

};

// ======================================================

// MATCHING

// ======================================================

function locationMatches(location)

{

    const f = filters.values();

    // Type

    if (f.type !== "" && f.type !== "Any")

    {

        if (getLocationType(location) !== f.type)

            return false;

    }

    // District

    if (f.district !== "" && f.district !== "Any")

    {

        const districts =

            Array.isArray(location.location)

                ? location.location

                : (location.location

                    ? [location.location]

                    : []);

        let found = false;

        for (const district of districts)

        {

            if (

                getLinkLabel(district)

                === f.district

            )

            {

                found = true;

                break;

            }

        }

        if (!found)

            return false;

    }

    // Affiliation

    if (f.affiliation !== "" &&

        f.affiliation !== "Any")

    {

        const affiliations =

            Array.isArray(location.affiliation)

                ? location.affiliation

                : (location.affiliation

                    ? [location.affiliation]

                    : []);

        let found = false;

        for (const affiliation of affiliations)

        {

            if (

                getLinkLabel(affiliation)

                === f.affiliation

            )

            {

                found = true;

                break;

            }

        }

        if (!found)

            return false;

    }

    return true;

}

// ======================================================

// EVENTS

// ======================================================

filters.type.onchange = refresh;

filters.district.onchange = refresh;

filters.affiliation.onchange = refresh;

// ======================================================

// RESULTS

// ======================================================

function computeResults()

{

    const results = [];

    for (const location of locationPages)

    {

        if (locationMatches(location))

        {

            results.push(location);

        }

    }

    results.sort((a, b) =>

        a.file.name.localeCompare(

            b.file.name,

            undefined,

            {

                sensitivity: "base"

            }

        )

    );

    return results;

}

// ======================================================

// TABLE DEFINITION

// ======================================================

table.addColumn(

    "Location",

    (cell, location) =>

    {

        renderWikiLink(cell, location);

    }

);

table.addColumn(

    "Type",

    (cell, location) =>

    {

        cell.setText(

            getLocationType(location)

        );

    }

);

table.addColumn(

    "District",

    (cell, location) =>

    {

        renderDistrict(cell, location);

    }

);

table.addColumn(

    "Affiliation",

    (cell, location) =>

    {

        renderAffiliations(cell, location);

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

        text: `${results.length} Locations found`

    });

    table.parent = resultPanel;

    table.render(results);

}

// ======================================================

// INITIAL RENDER

// ======================================================

refresh();

```