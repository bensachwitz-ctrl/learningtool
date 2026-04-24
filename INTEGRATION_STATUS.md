# Integration Status — Unified `swamp` App

The Learning Tool is integrated into the unified Swamp Fox Agency app at:

> **`bensachwitz-ctrl/swamp`** on branch
> **`claude/integrate-github-dashboard-gbFRU`**

It lives there under `/learningtool/` and launches from the dashboard's
topbar (single icon — the previous SFA-dash port rendered it twice; only
the topbar instance survives).

## What the `swamp` copy is (and isn't)

It is a **curated rebuild**, not a fork of this repo's generic deck.

- **Stripped** every entry tied to product lines Swamp Fox doesn't write
  (marine, aviation, crypto, NFT, pet, drone, etc.).
- **Added** SFA-specific terms: SCTPA, Alirics, the forestry carriers we
  actually appoint with, the SC-county-specific wind/hail deductible
  rules, the MCS-90 myth-busting, the Moncks Corner / Waycross office
  routing.
- **Expanded** to ~100 glossary terms + 12 playbooks + 10 deep-dives +
  30–40 external resource links, all mapped to real SFA workflows.
- **Wired** to the shared brand tokens at `/shared/brand.css` so it
  visually matches the dashboard and marketing site.

## Why keep this repo

This repo remains the generic / public reference for the underlying
Learning-Tool shell (the search + tab + card pattern). The `swamp` copy
is the canonical Swamp Fox edition — edits there, not here.

If another agency wants to adopt the shell for their own lines, they
fork THIS repo and swap in their own `data.js`.

## No code changes in this branch

This branch of `learningtool` carries docs only. The actual curated
content lives in the `swamp` repo on the matching branch.
