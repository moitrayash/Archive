# Archive

Public-facing archive for [yashmoitra.com](https://yashmoitra.com). Maintained.

Live at **https://archive.yashmoitra.com**

## Contents

- `index.html` — archive index
- `letter-to-residents/` — Letter to Residents (2025–26), Clara Dickson Hall & High Rise 5

## Adding an entry

Add a folder at the repo root with an `index.html`, then add one `.entry` row to
the relevant `<section>` in `index.html`:

```html
<div class="entry">
  <a href="/your-slug/" target="_blank" rel="noopener noreferrer"
     data-tip="One-line hover description">Title</a><span class="meta">Year</span>
</div>
```

New categories get their own `<section class="section">` with an `<h2>`.

## Notes

- Static. No build step, no dependencies. Served by GitHub Pages from `main`, `/ (root)`.
- `CNAME` pins the custom domain; do not delete it.
- Links are root-relative (`/letter-to-residents/`), so the site must be served
  from the domain root — not a subpath.
