```dataview
LIST
FROM "health"
```
```dataview
TABLE file.link, item.text  
FROM ""  
FLATTEN file.lists AS item  
WHERE item.section = "Health today"
```
```dataview
TABLE file.name AS Date, L.text AS Symptom  
FROM ""  
FLATTEN file.lists AS L  
WHERE L.section = "Health Today"  
SORT file.name DESC
```
