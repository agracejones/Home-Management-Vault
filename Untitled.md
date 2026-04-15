
```dataview
TABLE file.name AS Date, L.text AS Symptom  
FROM ""  
FLATTEN file.lists AS L  
WHERE regexmatch("Health Today", L.header)
```
```dataview
TABLE L.text, L.section  
FROM ""  
FLATTEN file.lists AS L  
WHERE contains(L.text, "Swollen")
```


