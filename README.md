# Ishaq Hamza: academic website

## What's in here
- `index.html`: the whole site (pages, styles, scripts).
- `assets/`: the portrait (WebP, with a PNG fallback).
- `cv/`: the two CV PDFs shown on the CV tab. `cv/source/` holds their LaTeX sources.
- `vendor/`: PDF.js, which draws the CVs so they fit the page in every browser.

## Putting it online (GitHub Pages, free)
1. Create a public GitHub repository named `IshaqHamza.github.io`.
2. Upload everything in this folder, keeping the folder structure.
3. In the repository, go to Settings → Pages, choose "Deploy from a branch", branch `main`, folder `/ (root)`.
4. After a minute the site is live at https://ishaqhamza.github.io

To preview on your own computer, run `python3 -m http.server` in this folder and open
http://localhost:8000. If you double-click `index.html` instead, everything works except
that the CV tab falls back to the browser's built-in PDF viewer.

## Editing
All content lives in `index.html`; search for these.
- **News**: the `<ul class="news">` list. Newest first; copy an `<li>` to add an item.
- **Papers**: the `<ol class="pubs">` list. Copy the `<li class="pub">` block for each new paper.
- **Presentations**: replace "To be updated." under the Presentations heading.
- **ResearchGate link**: marked with a `TODO` comment; check the URL.
- **Easter-egg quotes and jokes**: the `var quotes = [...]` and `var jokes = [...]` lists.
- **CVs**: edit the `.tex` file in `cv/source/`, compile it (e.g. on Overleaf), and replace the
  matching PDF in `cv/`, keeping the same file name.
- **Footer**: "Last updated …" at the bottom of the page.

## Credits
PDF.js (Apache 2.0, see `vendor/LICENSE-pdfjs.txt`). Brand icons from Font Awesome Free (CC BY 4.0).
