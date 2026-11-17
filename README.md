# welcome-tribute-075934 — optimised Framer export, GitHub-ready

Source: https://welcome-tribute-075934.framer.app/

A faster copy of the Framer export. Design, animations and page transitions are unchanged.

## Folder layout — every top-level folder has 80 files or fewer
```
(root)           index.html, styles.css, README.md, .nojekyll
about/           index.html   (page)
amenites/        index.html   (page)
contact/         index.html   (page)
site-plans/      index.html   (page)
fonts/           80 files
images-1/        79 files
images-2/        79 files
images-3/        77 files
js/              31 files
```
355 files in total. Every path in the HTML, CSS and JS points to these folders.

## Upload to GitHub on the website (no more than 100 files per upload)
1. Create a new repository.
2. **Upload 1:** choose *Add file → Upload files*, then drag in the root files (`index.html`, `styles.css`, `README.md`) and the page folders `about`, `amenites`, `contact`, `site-plans`. Commit.
3. **Upload 2:** drag in the `fonts` folder (80 files). Commit.
4. **Upload 3:** drag in the `images-1` folder (79 files). Commit.
5. **Upload 4:** drag in the `images-2` folder (79 files). Commit.
6. **Upload 5:** drag in the `images-3` folder (77 files). Commit.
7. **Upload 6:** drag in the `js` folder (31 files). Commit.

Drag each folder itself, not the files inside it, so GitHub keeps the folder name.
`.nojekyll` is a hidden file on Mac. If it didn't upload, create it with *Add file → Create new file*, name it `.nojekyll`, and leave it empty.

**Or use git / GitHub Desktop** (no file limit):
```bash
cd welcome-tribute-075934
git init && git add . && git commit -m "Initial upload"
git branch -M main
git remote add origin https://github.com/<you>/<repo>.git
git push -u origin main
```

**Go live:** Settings → Pages → Deploy from a branch → `main` / `(root)`. It works at `https://<you>.github.io/<repo>/`, and every page and link has been tested from a sub-folder address like that.

## What made it faster
- Images re-saved as WebP at the same pixel size, about 60% smaller
- Photos baked inside large SVG files compressed, and duplicate files merged
- Videos re-encoded to H.264 with fast-start, so they play everywhere and start sooner

## Preview locally
```bash
python3 -m http.server 8000   # then open http://localhost:8000
```
