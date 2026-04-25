---
kanban-plugin: board
project: BankBud
repo: https://github.com/auntiehomie/bankbud
priority: "1"
---

## Next

- [ ] - Build user memory/training into BankBud Chat
- [ ] - Add `FRED_API_KEY` to Render env vars (free key — fred.stlouisfed.org) [needs-manual::deploy env var on Render dashboard]


## In Progress


## In Review


## Backlog


## Done

- [x] - Fix rates loading issue [done::2026-04-12]
- [x] - Investigate reliable rates data source (replace Perplexity/Jina scraper approach) [done::2026-04-24]
- [x] - Add more news feed sources (finance, crypto, banking, savings) [done::2026-04-24]
- [x] - Reorder perplexityService.ts to call Jina BEFORE Perplexity for known bank URLs [done::2026-04-25]
- [x] - Add rate-fetch monitoring: log per-tier success/failure to see which banks need Perplexity [done::2026-04-25]

## Cancelled




%% kanban:settings
```
{"kanban-plugin":"board"}
```
%%
