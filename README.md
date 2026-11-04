# PlayLab Studio Card — academyEX

A standalone, client-side Studio Card builder for the Futures PlayLab. Students can reflect on what they explored, made or tested, what surprised them, what changed, and what they would do next; see a live preview; and export a high-resolution PNG.

## Publish on GitHub Pages

1. Create a **public GitHub repository** (e.g. `playlab-studio-card`).
2. Upload `index.html` to the **root** of the repository and commit it. No other files are required.
3. Open **Settings → Pages** in your GitHub repository.
4. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then **Save**.
5. Your site will be accessible at `https://YOUR-USERNAME.github.io/playlab-studio-card/` after GitHub finishes deploying. Use the URL shown under Settings → Pages.

## Features

- Includes the original academyEX logo embedded directly in the HTML.
- Live canvas preview of a polished five-part reflection card.
- Exports a detailed, high-resolution (2×) PNG, with automatic card height for longer answers.
- Autosaves in the same browser using `localStorage` (if available).
- **Save draft** downloads an editable `.json` file; **Open draft** restores it.
- Mobile and desktop responsive.
- No dependencies, user accounts, AI services, or data uploads.

## Student privacy and backups

Text is only held in the student's browser unless they export or save a draft. Browser storage may be cleared or unavailable in private mode, so students should **save a JSON draft** if they intend to return later. A PNG is an image and cannot be re-imported for editing. For a new public repository, remind students that the **website code** is public, but student responses are not submitted to GitHub.

## Customising

Everything is contained in `index.html`. You can change headings and prompts in the HTML; adjust card titles and accent colours in the `SECTIONS` JavaScript array; and customise fonts/colours in the CSS. The PNG uses the browser Canvas API, with the exact academyEX logo included in the card.

## Test locally

Double-click `index.html` to open it in a modern browser. It also works when published through GitHub Pages.
