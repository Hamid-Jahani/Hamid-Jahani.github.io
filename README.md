# Hamid-Jahani.github.io

Personal academic homepage, served at <https://hamid-jahani.github.io>.

Plain HTML and CSS with no build step, no framework, and no JavaScript beyond a
one-line footer year. `.nojekyll` tells GitHub Pages to serve the files verbatim
rather than running them through Jekyll.

```
index.html     the page
style.css      all styling; light and dark palettes share one rule set
assets/        images (add photo.jpg here)
```

## Adding a photo

Drop a square headshot at `assets/photo.jpg`, then in `index.html` replace the
`<div class="portrait-slot">…</div>` placeholder with:

```html
<img class="portrait" src="assets/photo.jpg" alt="Hamid Jahani">
```

## Local preview

```bash
python -m http.server 8000
# then open http://localhost:8000
```

Changes pushed to `main` publish automatically.
