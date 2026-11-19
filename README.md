# PlayLab Studio Card — academyEX

**Version 1.4 · For the full learning journey**

A lightweight, self-contained reflection tool for Futures PlayLab. Students use it whenever an activity, project, experiment or learning experience changes their thinking — not just for a particular workshop or day.

**Learning flow:** Learning experience → reflection → visible evidence → Digital Portfolio.

## What changed in v1.4

The previous **“Activities from today”** checkbox list has been replaced with a single free-text field: **“Activity or learning experience.”** Students can describe any workshop, class activity, independent project, experiment, feedback session or iteration. This description appears in the Studio Card preview and in every export.

The five core reflections remain unchanged:

1. What did you explore?
2. What did you make or test?
3. What surprised you or what did you notice?
4. What changed?
5. What would you do next?

The questions are general-purpose; guidance no longer depends on selected workshop activities. The project/focus, date and tools fields still provide context. An optional photo, screenshot, sketch, artefact reference or URL can be added as evidence. The Digital Portfolio connection is explicit.

### Export and draft options

| Action | Result |
|---|---|
| **Download PNG card** | High-resolution image with branding, activity description, five reflections and optional evidence |
| **Save as PDF** | Browser print-to-PDF with branded, colour card styling and **searchable/selectable text** |
| **Download text (.md)** | Editable Markdown containing the activity description, responses and evidence references |
| **Save draft / Open draft** | Portable JSON file for returning to an unfinished card, including an attached compressed image if present |

A current draft is also kept in this browser’s local storage when that feature is available. For important work, use **Save draft** before leaving the page. The draft storage key is unchanged from earlier versions.

### Compatibility with earlier cards

Students can import JSON drafts created with versions 1.1–1.3. Existing selected MAKE/EXPLORE activities are **converted to a readable activity description** in the new free-text field. The earlier reflections, student information, date, project focus, tools and evidence are retained. The same conversion happens for a previously saved draft in browser local storage on upgrade.

## Publish to GitHub Pages

1. Create or open the GitHub repository for the Studio Card.
2. Upload or replace `index.html` in the repository root.
3. Go to **Settings → Pages** and set **Deploy from a branch**, `main`, and `/ (root)`.
4. Visit the GitHub Pages address shown in repository settings.

For an existing site, **replace only `index.html`**. The site requires no build, bundler, account, API, external scripts or separate logo files.

## Notes on privacy and exporting

- All student data, images and exports are processed on the student's device. The site itself does **not** transmit submissions to academyEX or automatically upload to a Digital Portfolio.
- The academyEX landscape logo is embedded directly in `index.html`.
- Image evidence is compressed locally for reliable preview, PNG/PDF export and JSON draft saving.
- Students should choose **Save as PDF** in the browser print dialog. For browsers that show extra URL/date headers or omit backgrounds, disable **Headers and footers** and enable **Background graphics**.
- PDFs are generated from print-only HTML text, not by converting a screenshot. This keeps the body text searchable.
- On cards with very long reflections or large evidence, a multi-page PDF is expected.

## Verification

Checks completed in headless Chromium against the self-contained HTML: responsive layout, new activity entry, live preview, PNG and Markdown downloads, JSON export/import, legacy draft migration, PDF print DOM and searchable PDF text. A typical filled card exports as one A4 PDF page. Browser navigation and persistence cannot be tested against a hosted GitHub Pages origin in this sandbox; publishing and cross-browser checks should still be done on the live site.
