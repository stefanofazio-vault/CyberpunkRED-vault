```dataview
TABLE WITHOUT ID
    file.link AS "Location",
    file.folder AS "Categoria"
FROM "Locations"
SORT file.folder ASC, file.name ASC
```