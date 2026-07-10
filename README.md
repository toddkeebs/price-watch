# Price Watch

Personal price-tracking dashboard, updated daily by an automated Claude task.

**Dashboard:** https://toddkeebs.github.io/price-watch/

## How it works
- `data/watchlist.json` — items being tracked (name, group, target price, sites to check, image)
- `data/history.json` — daily price observations per item (`prices` = tracked sites, `deals` = deal-site/web finds)
- A scheduled task runs each morning at 7am: checks tracked sites, searches deal sites (dealsea, Slickdeals, etc.) and the web, appends results, and pushes.

## Adding items
Text yourself in Messages: `WATCH: item name, target $X` — picked up at the next daily run. Or ask Claude directly.
