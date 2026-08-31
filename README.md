# Hamid-Jahani.github.io

Personal academic homepage, served at <https://hamid-jahani.github.io>.

Plain HTML and CSS with no build step, no framework, and no JavaScript beyond a
one-line footer year. `.nojekyll` tells GitHub Pages to serve the files verbatim
rather than running them through Jekyll.

```
index.html     the page
style.css      all styling; light and dark palettes share one rule set
assets/photo.jpg  portrait, 480x480
```

## Adding a photo

`assets/photo.jpg` ships pre-cropped to a square (480x480, ~40 KB) framed on
the eye line. To replace it, drop a new source in `assets/` and re-run the crop
so the shipped file stays square and small.

## Local preview

```bash
python -m http.server 8000
# then open http://localhost:8000
```

Changes pushed to `main` publish automatically.
