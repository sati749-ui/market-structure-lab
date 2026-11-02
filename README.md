# Market Structure Lab

Premium, responsive Indian-equities research terminal. Buildless HTML, CSS and JavaScript: open index.html or serve the repository with any static HTTP server. No packages, build, remote fonts or credentials are required.

## Command Center

- Grouped sidebar and mobile navigation, candidate search (keyboard shortcut /), system status.
- Four sample KPIs; explicit Bullish / Neutral / Bearish regime vocabulary and explanation.
- Six chart periods with deterministic synthetic candles, illustrative structure and demand zone.
- Breadth, three-timeframe trend, sector period controls and relative-performance drill-downs.
- Setup filters, bullish/bearish tables, empty states, and stock research dialogs covering structure, order blocks, volume, RS, OI, events, evidence, risk, Devil's Advocate and Head of Desk.
- Market Summary. The former prototype is retained in legacy-research.html for reference.

## Data contract and remaining work

All displayed values and securities are synthetic examples, including familiar ticker names. Fixtures live in app.js. Period buttons change demonstration visuals; they do not request historical prices. The regime and structure labels are illustrative, not calculated signals.

Production requires licensed/authorized OHLCV inputs with source, exchange timestamp, adjustment policy and freshness state; market calendar; deterministic structure/order-block rules; breadth and sector benchmarks; scanner ranking; volume and derivatives data; event/corporate-action checks; validated backtests with costs and out-of-sample evidence; portfolio sizing and risk vetoes. Missing/stale inputs must display unavailable and must never fall back to these sample fixtures.

Evidence Lab, Risk Engine, Paper Trading and Journal navigation currently open honest status panels. Their engines are not implemented. No broker execution or secret/API key is included. Add credentials only in a future server-side service, never browser code.

## Verification

Run `node --check app.js`. Browser checks cover chart-period switching, sector drill-down, setup filtering, stock evidence, search/empty states, mobile navigation, dialog close/Escape, and responsive overflow. Serve locally for browser QA; no backend is needed.
