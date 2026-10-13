# geo-pdf-assets

Static assets for the GEO by Logarithmic PDF report: the report HTML template, subset web fonts and logos.

Used by the GEO by Logarithmic Grok Bot `geo-pdf-report` skill, which downloads these files from this repo at tag `v2`, checks each one against the sha256 values in `manifest.json` (stopping on any mismatch), fills the template and renders it to PDF with headless Chromium.

- `template.html`: report template (light theme), loads `fonts/` and `img/` by relative path.
- `fonts/`: Montserrat (400 to 800) and Instrument Serif Italic, Latin-subset woff2. Both fonts are licensed under the SIL Open Font License 1.1; see `fonts/OFL-*.txt`.
- `img/`: Logarithmic logo (light theme).
- `manifest.json`: sha256 of every asset.

Tags are never moved. A changed asset gets a new tag (v2, ...).
