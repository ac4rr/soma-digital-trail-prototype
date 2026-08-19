# Soma Digital — "Trail" design prototype

A single-page installable PWA design prototype for Soma Digital, a daily
spiritual discovery app. Six screens (Home, Devotional Detail, Kingdom
Scrolling, Connect, Pray, Settings) switched client-side with no page reload.

**This is a design prototype, not the production app.** All content is sample
data, defined in one `SOMA_SAMPLE_DATA` object at the top of the script in
`index.html`. There is no backend and no persistence; state is in-memory only.

## Stack

Plain HTML, CSS and vanilla JS in one file. No build step, no bundler, no npm
dependencies. Inter from Google Fonts. A `manifest.webmanifest`, a service
worker (`sw.js`) caching the shell and fonts for offline use, and local icon
assets drawn from the Soma Digital wordmark.

## Run

Serve the folder with any static server, e.g.:

```
python3 -m http.server 8080
```

## Open product question

The Home path implies a sequenced plan (21 days, "Peace", day 15 = today).
The production app has an independent devotional library with tabs and
search — no such sequence exists there yet. See the note above
`SOMA_SAMPLE_DATA` in `index.html`.
