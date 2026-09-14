# SYMFRA website

Source for [symfra.net](https://symfra.net) — the site of SYMFRA, an international
community advancing Symbiotic Infrastructure.

## Structure

```
index.html            the whole site (single page, four tabbed panels)
assets/logo.png       wordmark, dark — used in the header
assets/logo-white.png wordmark, white — used in the footer
```

There is no build step. `index.html` contains the markup, the CSS (in a `<style>`
block) and the tab logic (in a `<script>` block).

## Working on it locally

Open `index.html` in a browser, or serve the folder:

```
python -m http.server 8000
```

Then visit http://localhost:8000.

## Publishing

The site is served by GitHub Pages from the `main` branch, `/` (root).
Pushing to `main` publishes; it takes a minute or two to go live.

```
git add -A
git commit -m "Describe the change"
git push
```

## Content still to fill in

- Committee names and institutions (Committee) — nine `TBC` cards across the three
  groups. Replace the text and drop the `tbc` class from the card's `<div>`; that
  restores the normal green/blue initials styling.
- Member names, roles and institutions (About → Members) — currently placeholders,
  and overlapping with the Committee page
- Conference key dates (Conferences → Key dates) — currently "TBC"
- News entries — currently placeholders
