# CIS 4430 — GOV Personnel Information Exposure Lab, v1.6

GitHub Pages-ready, client-only GRC investigation workbench for Keiser University.

## What changed in v1.6

- Fixed and retested PowerPoint creation: output is generated as a Blob and offered as an `.pptx` download. The presentation archive passed ZIP validation in a local Node test.
- Replaced horizontally scrolling data-entry tables with labeled record cards for sources, applicability, IAM controls, evidence, risks, and POA&M. Inputs, selects, and date fields save on each edit.
- Made the three main actions contiguous: Submission Check, Print/Save PDF, and Export PowerPoint.
- Redesigned responsive academic banner and navigation with a vector banner background.
- Clarified **only required deliverable**: the final completed printed report (or PDF equivalent if the instructor accepts it). PowerPoint and workspace backup are optional.
- Preserved project autosave, backup, import, grading rubric, and all 10 investigation sections.

## Dedicated GitHub Pages address (new repository)

This package is prepared for a **new, separate public repository** named `cis4430-gov-personnel-lab`.

1. In GitHub, create a new **public** repository named `cis4430-gov-personnel-lab` under the `dragasakisn-beep` account. Do not initialize it with a README.
2. Extract this ZIP. Upload the **contents** of the package (including `index.html`, `app.js`, `styles.css`, `academic-banner.svg`, and the `vendor` directory) to the root of the new repository.
3. Commit the new files to branch `main`.
4. Open Settings → Pages → Deploy from a branch → `main` → `/ (root)` → Save.
5. The standalone Pages address will be `https://dragasakisn-beep.github.io/cis4430-gov-personnel-lab/` after publication.

**Do not replace any files in the existing `cis4430-grc-lab` repository.** Existing student backup files are compatible with the new application. Autosaved browser data is keyed under the original identifier to avoid losing existing work on migration.

## Release v1.6 fixes

- Version label displays **v1.6** with versioned script and stylesheet URLs to avoid stale browser caches.
- Last-section navigation now reads **Review submission checklist →** and opens validation instead of doing nothing.
- Submission validation, Print/Save PDF, and PowerPoint export are grouped together in a single contiguous action bar.
- Print layout includes the actual graphic banner using an image element, works even when background printing is disabled, and avoids the mostly blank opening page.
- PowerPoint export supplies a visible, repeatable **Save PowerPoint (.pptx)** link when the browser blocks automatic downloads.
- All ten investigation sections, student autosave, backup import/export, and instructor rubric remain intact.

## QA performed

- Node syntax check: passed.
- Functional unit check (text entry, selection, persistence callback, print HTML generation, validator): passed.
- Node PowerPoint generation test: passed; produced valid `.pptx` ZIP structure.
- Browser end-to-end testing: **not completed** because the test environment blocked browser navigation. On-site test is required, especially on Safari/in-app browsers, where automatic file downloads may be restricted.

## Privacy and data integrity

All entries are stored in the student's browser profile. No central server, instructor collection, login, or automatic grade submission. Do not enter live government records, credentials, or protected information.

The reported DHS information exposure provides an attributed research starting point. The FSSC scenario and its records remain fictional; the identity system intrusion claim is unverified.