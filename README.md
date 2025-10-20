# Image → WEBP Converter

A small, single-file web app that converts images to WEBP in the browser with simple controls for **quality** and **resize**. Designed to run locally or be hosted on GitHub Pages.

---

## Files

* `Image Webp Converter V4.html` — the single-file app (HTML + CSS + JS). Rename to `index.html` if you want GitHub Pages to serve it from the repository root.

## Features

* Local-only processing (no uploads to any server)
* Drag & drop or click-to-upload image input
* Validation: minimum 1 KB, maximum 5 MB
* Quality slider (50%–100% in 10% steps)
* Resize scale (10%–200% in 10% steps)
* Shows estimated percent reduction after conversion
* Download converted WEBP file

## Usage (local)

1. Open the HTML file in a browser (double-click `index.html` or `Image Webp Converter V4.html`).
2. Drop or choose an image.
3. Adjust Quality and Scale.
4. Click **Convert**, then click the **Download** button to save the WEBP.

## Deploy on GitHub Pages (quick)

1. Rename `Image Webp Converter V4.html` to `index.html` and commit it to your repo root.
2. In your repository on GitHub, go to **Settings → Pages**.
3. Under **Build and deployment**, choose the branch (e.g., `main`) and root `/` as the folder, then **Save**.
4. GitHub will provide a public URL once the site is published (usually within a minute).

### Deploy with Git (CLI)

```bash
# inside your project folder
git init
git add index.html README.md
git commit -m "Add webp converter"
git branch -M main
git remote add origin git@github.com:YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

Then enable Pages in the repo Settings as above.

## Notes & Tips

* For high-resolution images, use smaller scale or consider a backend (Node + `sharp`) for batch processing.
* This app relies on the browser's WebP encoder — older browsers may not support it.

## License

MIT — feel free to reuse and adapt.

---

If you want, I can:

* Rename the HTML to `index.html` and commit a small `gh-pages` branch for you,
* Add a screenshot to README,
* Provide the exact `git` commands tailored to your repository name.

Tell me which of those you'd like next.
