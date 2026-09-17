# Les Yeux Ouverts — Jekyll site

    bundle exec jekyll serve

## Where things live

- `_data/content.yml` — all copy, in `fr:` and `en:` blocks. Edit text here, not in the HTML.
- `_layouts/default.html` — page shell, fonts, FR/EN toggle script.
- `index.html` — section order and image placement.
- `assets/css/main.css` — all styling.
- `assets/img/`, `assets/fonts/` — images and Kunst Grotesk.

## Language

Both languages are rendered into the page; the toggle in the header shows one at a
time and remembers the choice in localStorage. No plugins needed. If you'd rather
have real `/` and `/en/` URLs later, the same data file can drive two pages.

## To confirm

- Publisher shop URL (currently `https://lecturis.nl`) — `_data/content.yml`, `order_url`.
- Contact email (currently `studio@jeremystigter.com`) — same file.
