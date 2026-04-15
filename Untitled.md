
```dataview
TABLE file.name AS Date, L.text AS Symptom  
FROM ""  
FLATTEN file.lists AS L  
WHERE L.header = "Health Today"  
SORT file.name DESC
```


```dataview
TABLE L.text, L.section  
FROM ""  
FLATTEN file.lists AS L  
WHERE contains(L.text, "Swollen")
```


