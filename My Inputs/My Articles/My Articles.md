---
tags: view/note
Links: "[[My Inputs]]"
Created: 2026-01-19T21:35:22
---

## By Status

### No Status

```dataview
table Created, Links, Source
FROM  #input/articles AND !"Hidden"
WHERE !Status
SORT started desc
```

### Not Started 🟥

```dataview
table Created, Links, Source
FROM  #input/articles AND !"Hidden"
WHERE contains(Status, "🟥")
SORT started desc
```

### Consuming Media 🟧

```dataview
table Created, Links, Source
FROM  #input/articles AND !"Hidden"
WHERE contains(Status, "🟧")
SORT started desc
```

### Implementation 🟨

```dataview
table Created, Links, Source
FROM  #input/articles AND !"Hidden"
WHERE contains(Status, "🟨")
SORT started desc
```

### Finished 🟩

```dataview
table Created, Links, Source
FROM  #input/articles AND !"Hidden"
WHERE contains(Status, "🟩")
SORT started desc
```

### Archived ⬛

```dataview
table Created, Links, Source
FROM  #input/articles AND !"Hidden"
WHERE contains(Status, "⬛️")
SORT started desc
```
