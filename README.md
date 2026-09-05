# IR Academy Pro

A single-file, offline-capable educational reference for Interventional Radiology (IR) procedures, aimed at IR fellows/residents, IR-certified technologists and nurses, medical students, and other healthcare professionals.

**Live site:** https://shadirawa-ship-it.github.io/IR-Academy-Pro/

## ⚠️ Review status — please read before relying on this content

This project is under active development and **has not yet completed a formal clinical review**. Procedure descriptions, device specifications, and protocol steps were drafted with AI assistance and have not been independently verified by a credentialed Interventional Radiologist, nursing/technologist representative, pharmacist, or medical physicist.

**Do not treat any figure, dose, threshold, device dimension, or compatibility statement in this application as clinically verified.** Always follow your institution's protocols and the current manufacturer Instructions For Use (IFU). See the in-app **Safety & Compliance** tab for the full disclaimer.

If you are a qualified reviewer (board-certified IR physician, IR nurse/technologist, pharmacist, or medical physicist) and would like to help review this content, please reach out via the contact below.

## What this is

- A **static, self-contained HTML file** (`index.html`) — no build step, no backend, no external data calls (enforced by a strict Content-Security-Policy).
- A structured library of **51 IR procedures** across four specialty areas (Neuro, Vascular, General, Oncology), each with a 7-section reference (Anatomy, Protocol, Devices, Variants, Complications, Nursing, Clinical Notes) where available.
- Supporting tools: a device-compatibility reference, a printable pre-procedure checklist, a materials/specifications catalog, and safety/workflow reference sections.
- Full-text search across every procedure and tool, generated automatically from a single canonical data source so it cannot drift out of sync with the procedure cards.
- Keyboard-accessible navigation, a focus-trapped reference modal, `prefers-reduced-motion` support, and light/dark themes.
- Deep-linkable sections and procedures via the URL hash (e.g. `#onc` or `#onc-11`) — links can be bookmarked or shared and will restore the same view.

## What this is not

- **Not a medical device** and not a substitute for clinical judgment, institutional protocols, or manufacturer IFU.
- **Not a certification or credentialing tool.**
- **Not a clinical decision support system** — it has no patient-specific logic.
- Not intended for use by the lay public.

See the in-app Safety & Compliance tab for the complete list of disclaimers and known limitations.

## Data collection

None. This is a static file with no analytics, tracking, or network calls beyond loading the page itself. Theme preference and the currently active tab are stored only in your own browser (`localStorage`/`sessionStorage`) and are never transmitted anywhere.

## Project structure

```
index.html      # The entire application (HTML + CSS + JS, single file)
README.md       # This file
SECURITY.md     # Vulnerability/error reporting process
LICENSE         # License terms
CHANGELOG.md    # Version history
```

## Running locally

No build step is required — open `index.html` directly in a browser, or serve the directory with any static file server, e.g.:

```bash
python3 -m http.server 8000
```

## Contributing / reporting an issue

Please report factual or clinical inaccuracies, accessibility problems, or bugs by opening a GitHub issue or emailing **shadirawa@gmail.com**. Clinical-content corrections are the highest priority and should ideally include a citation to a current guideline or primary source.

## License

See [LICENSE](./LICENSE).

## Changelog

See [CHANGELOG.md](./CHANGELOG.md).
