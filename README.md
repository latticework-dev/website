# latticework.in

Single static page. No framework, no build step, no dependencies.

- `index.html` — the whole site. CSS and JS inline.
- `CNAME` — custom domain for GitHub Pages.

The only runtime network call is a fetch to Horizon for the transaction in the
hero, and the page renders completely without it: the static values in the
markup are the same values the fetch returns, so a failed or slow request
changes nothing a visitor sees.

## Local preview

    python3 -m http.server -d . 8000

## Notes

Fonts are Google Fonts (IBM Plex Mono, Instrument Sans), ~88 KB for the latin
subsets. No analytics, no third-party scripts, no cookies.
