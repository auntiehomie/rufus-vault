# Projects Dashboard

## Active Work
```dataview
TASK
FROM "backlogs"
WHERE section = "Next" OR section = "In Progress"
WHERE !completed
SORT file.name ASC
```

## Health Table
```dataview
TABLE
  length(filter(file.tasks, (t) => t.section = "Next" AND !t.completed)) AS "Next",
  length(filter(file.tasks, (t) => t.section = "In Progress" AND !t.completed)) AS "In Progress",
  length(filter(file.tasks, (t) => t.section = "Backlog" AND !t.completed)) AS "Backlog"
FROM "backlogs"
SORT file.name ASC
```
