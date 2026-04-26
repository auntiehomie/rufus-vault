---
kanban-plugin: board
project: BankBud
repo: https://github.com/auntiehomie/bankbud
priority: "1"
last worked: 2026-04-26
---

## Next

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
- [x] - Build user memory/training into BankBud Chat [done::2026-04-26]
- [x] - Delete stale 3.65% APY phantom rates (purgeStaleRates on startup + daily cron) [done::2026-04-26]
- [x] - Designate account type when populating rates (migrateRateTypes on startup, classifier guards) [done::2026-04-26]
- [x] - Add news feed sources: CoinDesk, Financial Times, CNBC Finance, Motley Fool [done::2026-04-26]
- [x] - Slim navbar / fix BankBud Chat visibility (Header padding 1rem→0.5rem, dynamic chat height) [done::2026-04-26]

## Cancelled




%% kanban:settings
```
{"kanban-plugin":"board"}
```
%%
