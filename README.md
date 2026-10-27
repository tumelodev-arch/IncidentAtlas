# Incident Atlas

A local incident coordination and review log for severity, impact, response notes and follow-up.

**Live demo:** https://tumelodev-arch.github.io/IncidentAtlas/

## What it does

- Create, edit and delete incident records.
- Record service, severity, start time, impact and response notes.
- Resolve or reopen incidents, then search and filter by severity or state.
- Review open/P1 counts, monthly resolutions and median resolution duration.
- Export incident records as JSON and persist them in browser storage.

## Run locally

Open `index.html` in a modern browser. The application uses local HTML, CSS and JavaScript and has no build step or external runtime dependency.

## Data and privacy

Records stay in the current browser until exported or cleared. They are not sent to a server or shared across browsers. This is an incident-review practice tool, not a monitoring agent, alert router, paging service or shared system of record. It has no server, notifications, authentication or team storage. Use invented data only.

## Tests

The repository includes Playwright end-to-end tests. Install dependencies and Chromium before running them.

```bash
npm install
npx playwright install chromium
npm run test:e2e
```

## Interface design

The interface uses the shared Engineering Field Notes design language, adapted for this app's main task. Primary controls have labelled actions, the mobile layout keeps actions reachable, and keyboard focus is visible. The app uses its own accent colour to make it recognisable beside the portfolio.

## Limitations

This is a browser-based practice application. A successful static deployment does not establish that it has a backend, authentication, shared state or production monitoring.
