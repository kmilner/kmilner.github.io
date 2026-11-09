# Kevin Milner's academic website

A small, responsive website for GitHub Pages. Plain HTML and CSS; no build step,
JavaScript, external fonts, or dependencies.

## Editing

Edit `index.html` to update the biography, Tamarin prover description, and
publication profile links. Keep the page title and description in the `<head>`
consistent with the visible content.

- Publications link directly to DBLP and Google Scholar, so there is no separate
  bibliography to maintain here.
- To include a CV, add `assets/cv.pdf` and a link to it in `index.html`.
- Adjust colours, fonts, and spacing in `styles.css`.

## Preview locally

From this directory, run:

```sh
python3 -m http.server 8000
```

Open <http://localhost:8000>. Stop the server with Ctrl+C.

## GitHub Pages

Commit and push the website files to the branch used by GitHub Pages. In the
repository's **Settings → Pages**, use **Deploy from a branch**, select that
branch, and select **/ (root)**. The site is intended to be served at
<https://kmilner.github.io/>.

The `.nojekyll` file makes this a plain static site. No custom workflow or package
installation is required.
