# jeremystigter.com — Jekyll site

    jekyll build      # or: bundle exec jekyll serve

## What this site is

`jeremystigter.com` is Jeremy Stigter's site. The homepage is currently given over
almost entirely to one book, *Les Yeux Ouverts / With Open Eyes* — the header carries
the name, and "Jeremy Stigter presents / présente" sits above the book title. When
there is a next book, that line stays and the title under it changes.

Page order: cover & title → 01 The book → portrait → Photographs → 02 Jeremy Stigter
(bio + Other books) → 03 Specifications & order → 04 Contact.

## Where things live

- `_data/content.yml` — all copy, in `fr:` and `en:` blocks. Edit text here, not in the HTML.
- `_layouts/default.html` — page shell, head/OG metadata, FR/EN toggle script.
- `index.html` — section order and image placement.
- `assets/css/main.css` — all styling.
- `assets/img/`, `assets/fonts/` — images and Kunst Grotesk.
- `assets/favicon.svg` — placeholder mark (black square, "JS"). Replace when there's a real one.
- `CNAME` — the custom domain for GitHub Pages.

## Language

Both languages are rendered into the page; the toggle in the header shows one at
a time and remembers the choice in localStorage. No plugins needed. If you'd rather
have real `/` and `/en/` URLs later, the same data file can drive two pages.

Note that `<title>`, `<meta description>` and the Open Graph tags are emitted in
English and only the first two are swapped by JS — crawlers and link previews will
see English. Real per-language URLs would fix that properly.

## To confirm

- Publisher shop URL (currently `https://lecturis.nl`) — `_data/content.yml`, `order_url`.
- Contact email (currently `studio@jeremystigter.com`) — same file.
- Point the `jeremystigter.com` DNS at GitHub Pages and enable HTTPS in repo settings.
