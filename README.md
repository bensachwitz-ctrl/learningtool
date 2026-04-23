# Swamp Fox Insurance Knowledge Tool

An internal reference and learning tool for the team at Swamp Fox Insurance Agency. A single-file HTML web app that works offline, on any device, with no install required.

<p align="center">
  <img src="https://img.shields.io/badge/type-single--file_web_app-1F4645" alt="Single-file web app">
  <img src="https://img.shields.io/badge/install-none-1F4645" alt="No install">
  <img src="https://img.shields.io/badge/glossary-641_terms-C8553D" alt="641 terms">
  <img src="https://img.shields.io/badge/reference_cards-914-C8553D" alt="914 cards">
</p>

## What's in it

- **Glossary** — 641 insurance terms, defined in plain English, spanning:
  - Core coverage types (auto, home, life, health, business, commercial)
  - Specialty lines (cyber, D&O, EPLI, kidnap & ransom, pollution, marine)
  - Commercial auto (Business Auto Coverage Form, all 11 covered-auto Symbols, Garage, Trucker, Motor Carrier forms, MCS-90)
  - Risk management (ERM, ISO 31000, COSO, Risk Equation, KRIs, residual risk)
  - Loss control & safety (OSHA, hierarchy of controls, JHA, LOTO, PPE, fall protection, hot work, fire protection, COPE)
  - Trucking safety (FMCSA, CSA, HOS, ELD, BASICs, DOT numbers, FMCSA Clearinghouse)
  - Logging & forestry (felling, bucking, yarding, skidding, danger trees, widowmakers, chain shot, state forestry codes)
  - Claims terminology (subrogation, IBNR, LAE, loss triangles, proximate cause)
  - Regulatory (NAIC, admitted vs. non-admitted, SAP, GAAP, RBC, state guaranty funds)
  - Contract risk transfer (hold-harmless, additional insured, waiver of subrogation, OCIP/CCIP)
  - Agency operations (book of business, contingent commission, MGAs, wholesale brokers)

- **Reference Section** — 914 conceptual reference cards organized by topic, for deeper learning on specific subjects.

## How to use

1. Open `index.html` in any modern browser — no server, no install.
2. Type any term in the search bar. Results appear instantly across both the glossary and reference section, with matches highlighted.
3. Use the A–Z bar in the glossary to jump directly to any letter.
4. Use the sidebar to browse by topic.

### Keyboard shortcuts

| Key | Action |
|---|---|
| `/` | Focus the search bar from anywhere |
| `Ctrl` + `K` or `⌘` + `K` | Focus the search bar |
| `Esc` | Clear the search and unfocus |

### Works on any device

Responsive layout adapts to phones (≥375px), tablets (≥768px), and wide desktop monitors (up to 1920px+). Glossary flows into 1, 2, or 3 columns depending on screen width.

## Structure

```
.
├── index.html          # The tool itself — open this in a browser
├── glossary.json       # The glossary data (641 terms)
├── reference.json      # The reference card data (914 cards)
├── README.md           # This file
└── LICENSE             # MIT License
```

The HTML file is fully self-contained — the JSON files are included only for transparency and future maintenance. You do not need them to use the tool.

## Hosting on GitHub Pages

To make this available to the team via a shareable link:

1. Push this repo to GitHub.
2. In the repo on GitHub, go to **Settings → Pages**.
3. Under "Source," select **Deploy from a branch** → **main** → **/ (root)**.
4. Your tool will be available at `https://<username>.github.io/<repo-name>/`.

## Updating

The three data sources and the build scripts are not included in this repo (to keep the distribution lean), but the structure of additions is straightforward:

- To add a glossary term, append an entry to `glossary.json`:
  ```json
  {
    "term": "New Term",
    "definition": "The definition in plain English."
  }
  ```
- To add a reference card, append to `reference.json` following the existing pattern.
- The HTML tool loads its content from embedded data at build time, so any changes to JSON need a rebuild.

## Scope

This is an internal reference tool. The content is drawn from publicly available insurance education materials, industry glossaries, and standard terminology. It is not a substitute for professional licensing education, state-specific legal advice, or coverage opinions on any specific risk.

---

© Swamp Fox Insurance Agency — Internal use
