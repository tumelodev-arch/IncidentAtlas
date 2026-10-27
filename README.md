# Incident Atlas

A local incident coordination and review log for recording severity, impact, response notes and follow-up.

## Demo

**Live demo:** [Open Incident Atlas](https://tumelodev-arch.github.io/IncidentAtlas/)

The GitHub Pages deployment workflow has reported success. The demo is a static browser app; records remain in the current browser and are not sent to a backend. A successful deployment is not a substitute for manual browser and accessibility checks.

**Run locally:** open `index.html` in a modern browser. The app has no build step or external runtime dependency.

## Features

- Create, edit and delete incident records.
- Record service, severity, start time, impact and response notes.
- Mark incidents resolved or reopen them.
- Search and filter by state and severity.
- Calculate open/P1 counts, current-month resolutions and median resolution duration.
- Export the incident log to JSON.
- Persist data in browser local storage.

## Run locally

Open `index.html` in a modern browser. There is no build step or external runtime dependency. `styles.css` and `app.js` are loaded locally.

## Data and privacy

Records are stored in this browser only; they are not sent to a server or shared across browsers. Use synthetic or non-sensitive information. Clearing browser storage can remove locally saved records.

## Boundaries

This is an incident-log practice tool, not a monitoring agent, alert router or on-call platform. It has no server, integrations, notifications, authentication or shared team storage. Do not paste credentials, customer information, production hostnames or sensitive incident details into this public demo.
