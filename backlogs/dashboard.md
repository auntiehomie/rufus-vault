# Projects Dashboard

## Health Table

```dataview
TABLE
FROM "backlogs"
WHERE file.name != "dashboard"
SORT file.name ASC
```

## Active Work

```dataview
TASK
FROM "backlogs"
WHERE file.name != "dashboard"
SORT file.name ASC
```
