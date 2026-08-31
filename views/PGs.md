```dataview
	TABLE WITHOUT ID
	    file.link AS "PG",
	    file.mtime AS "Ultima modifica"
	FROM "PGs"
	WHERE file.name != "PGs"
	SORT file.name ASC
```
