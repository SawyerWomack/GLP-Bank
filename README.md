# GLP Bank

A static, browsable archive of General Leadership Problems, sorted by run time.

## Files
- `index.html` — the site itself
- `glp-data.js` — the list of GLPs (title, time, group size, summary, and which PDF it links to)
- `glp-files/` — the individual GLP write-ups as PDFs

## Run it locally
Just open `index.html` in a browser — no server or build step needed.

## Host it free on GitHub Pages
1. Create a new repository on GitHub (public).
2. Upload all the files in this folder (`index.html`, `glp-data.js`, and the `glp-files/` folder), keeping the same structure.
3. Go to the repo's **Settings → Pages**.
4. Under "Build and deployment", set **Source** to "Deploy from a branch", pick the `main` branch and `/ (root)` folder, then Save.
5. GitHub gives you a URL like `https://yourusername.github.io/your-repo-name/` — that's your live site, updates automatically whenever you push changes.

## Add a new GLP
1. Drop the write-up as a PDF into `glp-files/`.
2. Open `glp-data.js` and add an entry to the list, e.g.:
```js
{
  "number": 42,
  "title": "Your GLP Title",
  "time_raw": "20 min",
  "time_minutes": 20,
  "group_size": "8-12 cadets",
  "location": "",
  "summary": "One or two sentence description of the exercise.",
  "file": "glp-files/042-your-glp-title.pdf"
}
```
3. Commit and push. GitHub Pages updates within a minute or two.
