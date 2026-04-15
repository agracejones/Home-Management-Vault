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
