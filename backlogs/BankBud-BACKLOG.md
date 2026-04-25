---

kanban-plugin: board
project: BankBud
repo: https://github.com/auntiehomie/bankbud
priority: "1"
last worked: 2025-01-01

---

## Next

- [ ] - Build user memory/training into BankBud Chat
- [ ] delete the stale 3.65% APY rates that keep showing up.  its showing every bank as 3.65%, no other actual rates. these rates are definitely wrong
	
	![[Pasted image 20260423191720.png]]
- [ ] when populating rates,  designate the type of account that the rate is connected to
- [ ] look for news feed sources from the financial times,coindesk,cnn finance, yahoo finance, and more.  news articles are only populating with a mention of the federal reserve.
- [ ] bankbud chat conversation is not fully visible],  when clicking the bankbud chat tab,  the screen should be fully visible.  make the navbar at the top of bankbud thinner so you can see the entire chat conversation screen when talking to bankbud chat.![[Pasted image 20260423191618.png]]
- [ ] ![[Pasted image 20260423191516.png]]the top bar seems to be too large.  i'd like for it to be more streamlined with the way that the app looks
- [ ] ![[Pasted image 20260425125408.png]] rates are now showing as unavailable.
- [ ] ![[Pasted image 20260425125445.png]] bankbud chat isnt completely visible when asking a question.  the way the page looks here is just off.  need to resize the header area in order to see the entire chat to make sure i can see the actual bankbud chat.
- [ ] having touble correctly tagging news articles.  ![[Pasted image 20260425125626.png]] the article showing looks to be best tagged under savings, not necessarily federal reserve


## In Progress

- [ ] - Add `FRED_API_KEY` to Render env vars (free key — fred.stlouisfed.org) [needs-manual::deploy env var on Render dashboard]


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