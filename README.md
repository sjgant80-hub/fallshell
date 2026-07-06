# FallShell

**One shell for the entire AI-Native Solutions estate.**

FallShell is a sovereign single-file PWA portal. Every shipped estate tool sits in a left sidebar, categorized. Click a tool — it loads in an iframe in the main pane. A collapsible right sidebar runs the foldkit overlay live: type into it, get a κ band, an op, and a probe. Your F(S⃗) fingerprint accumulates over time.

Live: <https://sjgant80-hub.github.io/fallshell/>

## What it does

- **Portal.** Twelve tools across Insight, Substrate, Signal, and Ops categories. Filter by name. Click to load.
- **Iframe by design.** Every tool renders inside the shell — no external navigation possible. The sovereign constraint holds.
- **Foldkit sidebar.** Live κ classifier + op picker + probe suggestion + F(S⃗) fingerprint tracker.
- **PWA installable.** One click to install as a desktop app (Chrome / Edge). Works offline for the shell itself; tools still need a network.
- **Local only.** IndexedDB stores your last tool, sidebar collapse state, and classification history. Nothing leaves the device except the tool iframes themselves.

## Keyboard

- `Ctrl+K` — open the search modal
- `Ctrl+B` — toggle the left sidebar
- `Ctrl+1` through `Ctrl+9` — jump to visible tools 1–9

## Layout

- **Top bar** — brand, install PWA button, sidebar toggles.
- **Left sidebar** — filter box, tools grouped by category. Private tools show a small ● dot.
- **Main pane** — welcome grid on load; switches to iframe once a tool is picked. Header shows tool name, category, URL, and an external-open link.
- **Right sidebar** — foldkit panel with three tabs: κ classify, F(S⃗), history.

## Tools included

**Insight** — FallMirror, Bloom Profile Builder, Bloom-weighted si-didy, 9-Axis Human Sonar.
**Substrate** — foldkit, κ-EEG Checker, INIT Book.
**Signal** — FallSignature, Mesh 89 Tracker, Hello Device, Quine Cube Runner.
**Ops** — FallPx.

## Files

- `index.html` — the shell (under 900 lines, one file).
- `foldkit.js` — origami-math ISA module (imported by the shell).
- `manifest.webmanifest` — PWA install manifest.
- `sw.js` — service worker; caches the shell for offline. Iframed tool requests pass through untouched.
- `.nojekyll` — GitHub Pages: serve raw.

## Sovereignty

Nothing leaves this device except iframe traffic to the tool pages themselves (which are on GitHub Pages, same estate). No analytics. No telemetry. No login. Your foldkit classification history sits in your browser's IndexedDB and nowhere else.

## License

MIT.
