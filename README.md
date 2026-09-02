# Discord Timestamp Generator

Generate Discord timestamps that render in every reader's local timezone. All 7 formats with live previews and one-click copy.

Live: <https://crusher-labs.github.io/discord-timestamp-generator/>

## What it does

Pick a date and time (or paste a raw Unix timestamp), and copy any of Discord's 7 timestamp formats (`<t:UNIX:letter>`): short/long time, short/long date, date + time, full, and relative. Quick presets for Now / In 1 hour / Tonight / Tomorrow / In 1 week; the relative preview updates live.

## Privacy

This tool runs entirely in your browser. There is no server. No data is uploaded, no telemetry, no analytics. The only network requests fired are the page-load fetches for the framework's CSS / JS (from `cdn.jsdelivr.net` and `fonts.googleapis.com` / `fonts.gstatic.com`); your inputs and outputs never leave the tab.

## Framework / hosting

- Static HTML / CSS / JS deployed via GitHub Pages from this repo's `main` branch.
- UI chrome is the published `crusher-ui-kit` static contract; the pinned version and its SRI hashes are managed fleet-wide by `tools-hub/scripts/bump-kit.mjs`.

## Development

- Open `index.html` directly in a browser. No build, no dependencies.
- Or serve the parent workspace via the hub's preview server: `cd ../../tools-hub && npm run preview` then visit `http://127.0.0.1:8723/utility-tools/discord-timestamp-generator/`.

## License

MIT.
