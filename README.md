# PlayLab Studio Card — academyEX

**Version 1.2 · Futures PlayLab**

A self-contained, accessible, mobile-friendly web tool that helps academyEX learners make studio learning visible. The goal is not simply to document an activity, but to **capture how thinking changes through making, testing and reflection**.

**Learning flow:** Studio activity → reflection → visible evidence → Digital Portfolio.

## Student experience

1. Select one or more MAKE / EXPLORE activities from the workshop. Relevant hints appear beneath the five questions.
2. Optionally add your name, date, project focus and tools.
3. Complete **one Studio Card** with the same five reflections for everyone:
   - What did you explore?
   - What did you make or test?
   - What surprised you **or what did you notice**?
   - What changed? (especially in your thinking or assumptions)
   - What would you do next?
4. **Optional evidence:** Describe an artefact or local file, paste a prototype/file URL, and/or attach one photo, screenshot or sketch. Uploaded images appear on the exported card. No extra reflection questions are required.
5. Export the card and add it to your **Digital Portfolio** as evidence of an experiment, iteration or shift in thinking.

### Workshop activities

- **MAKE 1 — System → Intervention:** Map a real context/system, identify a relationship or friction point, create a low-fi intervention.
- **MAKE 2 — Cybernetic / Adaptive Redesign:** Analyse feedback, control and system response, adapt the intervention into V2.
- **MAKE 3 — PlayLab Google Site Challenge:** Redesign part of the digital PlayLab home for participation, exploration and contribution.
- **EXPLORE 1 — Collective Frame VR:** Explore shared spatial experience through a 4E+/enaction lens.
- **EXPLORE 2 — VR Headsets:** Experience VR affordances, movement and interaction.

## Export options

| Option | What it does | Best for |
|---|---|---|
| **Download PNG card** | Creates a high-resolution, academyEX-branded image. The canvas grows to accommodate longer answers and optional evidence images. | Visual Digital Portfolio entries, sharing and presentation |
| **Save as PDF** | Opens your browser's print dialog with a clean, print-optimised document; choose **Save as PDF**. Text remains selectable/searchable and images are included. | Searchable portfolio archives and assessment records |
| **Download text (.md)** | Saves the card's written content and any evidence reference/URL as Markdown text. Embedded images are *not* carried into this text file. | Copying, editing and searching reflection text |
| **Save draft / Open draft** | Downloads or imports a JSON file with all current fields, selected activities and any compressed evidence image. | Returning to unfinished cards or moving devices |

**Tip:** PDF is created through your browser's built-in *Print → Save as PDF* option. No third-party PDF service or account is involved.

## Publish to GitHub Pages

1. Create a public repository, e.g. `playlab-studio-card`.
2. Upload `index.html` to the repository root (and optionally this README).
3. Under **Settings → Pages**, choose **Deploy from a branch**; select `main` and `/ (root)`.
4. Open the URL GitHub displays, typically `https://YOUR-USERNAME.github.io/playlab-studio-card/`.

To upgrade an existing v1.0 or v1.1 deployment, **replace the old `index.html` with the new one**. Existing locally stored text and activity selections are retained where they exist. Old JSON drafts also remain importable.

## Privacy and technical details

- This is a static HTML/CSS/JavaScript app. There are no external libraries, fonts, CDN requests, API keys, analytics or databases.
- No student content, photos or URLs are uploaded by this website. Responses and image data are processed locally on the device.
- Data is stored in browser `localStorage` when available. Storage can be cleared by the browser or blocked, so **Save draft** is recommended for important work.
- Uploaded images are converted to a smaller JPEG in the browser (one image per card) for reliable PNG, PDF and JSON exports. Animated GIFs are captured as a single frame.
- PDF text is rendered as real HTML text, not as an image. PDF printing depends on the browser; the student chooses the final save destination.
- Exports are local files only. Students must upload their Studio Card to their own Digital Portfolio; the tool does not upload it automatically.
- `index.html` is the entire deployable website; the original academyEX landscape logo is embedded in it.
