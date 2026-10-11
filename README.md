# From Architecture to Production — Nipun David

A static GitHub Pages portfolio using the **Engineering Fieldnotes** blueprint theme: off-white technical canvas, navy structural lines, violet accents, monospaced annotations, and original SVG schematics.

## Structure

- `index.html` — homepage and project/notes index
- `work/` — five case studies (NEOM simulation, Text-to-SQL, composable SDKs, enterprise RAG)
- `notes/` — engineering notes archive and LLM cascading report page
- `assets/css/styles.css` — shared responsive design system
- `assets/js/main.js` — mobile navigation
- `assets/illustrations/` — editable SVG diagrams and favicon
- `assets/docs/llm-cascading-report.pdf` — supplied PDF report

## Preview locally

Open `index.html` in a browser. For a local server, run:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000` from the project directory.

## Publish with GitHub Pages

1. Create or open the repository used for your GitHub Pages site (for a user site, it is usually named `USERNAME.github.io`).
2. Copy the **contents** of this folder into the repository root. Keep `index.html` at the root.
3. Commit and push to the branch configured for Pages (commonly `main`, `/root`).
4. In GitHub: **Settings → Pages**, confirm the source branch and root folder.
5. After deployment, test the home page, each case study, all note links, and the PDF on desktop and mobile.

No build step, Node.js, backend, or framework is required.

## Editing and adding content

- Add a new project page under `work/`, link it from the project grid in `index.html`, and reuse the `.page-main`, `.schematic-panel`, `.article-layout`, and `.side-panel` classes.
- Add an SVG under `assets/illustrations/` and reference it with a relative path.
- Add a note row to `notes/index.html` and optionally feature it on the homepage.
- Use relative paths (`../assets/...`) on nested pages so the site works under GitHub Pages project or user sites.
- Motion respects `prefers-reduced-motion`. Keep important information readable with animations disabled.

## Accuracy and confidentiality

The case studies are based on project experience and documented outcomes. Client/company details are kept high-level; diagrams are illustrative and do not reproduce client assets. Check that every detail is approved for public disclosure before publishing. Employer and internal platform names are omitted from the orchestration case study. No Genie Studio project is included.
