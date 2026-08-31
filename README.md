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

Save the headshot as `assets/photo.jpg`, commit, and push. No HTML change is
needed — the page already points at that path.

The image does not have to be square. It is cropped by CSS with
`object-fit: cover` and `object-position: center 22%`, which biases the crop
window toward the top of a tall portrait so the face stays centred instead of
the chest. If a different source photo crops badly, adjust that percentage in
`style.css`.

Until the file exists the image removes itself and a dashed placeholder shows in
its place, so the page never renders a broken-image icon.

## Local preview

```bash
python -m http.server 8000
# then open http://localhost:8000
```

Changes pushed to `main` publish automatically.
