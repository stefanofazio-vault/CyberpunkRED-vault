```dataview
TABLE WITHOUT ID
    file.link AS "Faction",
    file.folder AS "Categoria"
FROM "Factions"
SORT file.folder ASC, file.name ASC
```