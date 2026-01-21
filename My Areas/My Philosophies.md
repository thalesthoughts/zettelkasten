---
tags:
  - area
Links:
  - "[[My Areas]]"
Created: 2026-01-19T23:01:09
areaGroup: Personal
---
## Queries
### Projects

```dataview
table Status
FROM #project AND [[]] AND !"Hidden"
WHERE icontains(file.frontmatter.Area, this.file.name)
SORT Created asc
```
### Inputs

```dataview
table Status, Author
FROM  #input AND [[]] AND !"Hidden"
SORT file.mtime desc
```
### Other Notes

```dataview
table Created
FROM [[]] AND !#project AND !#input AND !"Hidden"
SORT file.mtime desc
```