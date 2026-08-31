```dataview
TABLE WITHOUT ID
    file.link AS "NPC",
    file.folder AS "Affiliation / Classe"
FROM "NPCs"
SORT file.folder ASC, file.name ASC
```