# Pickleball Black Friday and Cyber Monday Deals

A small static page of pickleball deals (paddles, bags, shoes, and accessories) with prices, promo codes, and spec dials for the paddles.

**Live site:** https://sidyadav3.github.io/pickleball-deals/

## Features

- One-tap copy buttons for promo codes
- Spec dials (power, spin, swing, and feel) for each paddle
- Light and dark mode, with a toggle in the header
- Responsive layout that works on phones and desktops
- No build step, frameworks, or dependencies

## Project structure

```
pickleball-deals/
├── index.html      # The whole page: HTML, CSS, and a little JavaScript
├── images/         # Product photos used on the page
└── README.md
```

## Editing the page

Everything lives in `index.html`.

- **Prices, codes, and copy:** edit the text inside the matching `<article>` block.
- **Links:** each product name and retailer is a standard `<a href="...">` tag.
- **Colors:** the palette is defined as CSS variables at the top of the `<style>` block (`:root`). Dark mode values are in the two `prefers-color-scheme` and `data-theme="dark"` blocks below it.
- **Dials:** each paddle has a `<div class="dials">` section. Gauge needles are SVG polygons, and the feel markers are positioned with a `left` percentage (for example, `left:32.5%`).
- **Images:** add or replace files in `images/` and update the matching `<img src="images/...">` path.

To publish a change, commit it to the `main` branch. GitHub Pages redeploys in a minute or two.

## Hosting

The site is served with GitHub Pages from the `main` branch, root folder (Settings → Pages → Deploy from a branch).

## Credits and disclosures

- The paddle promo codes are affiliate codes. The page owner earns a small commission when they're used.
- Dial readings are based off [John Kew Pickleball](https://www.johnkewpickleball.com/).
- Product photos belong to their respective brands and retailers and are used here for sharing deals with friends.
- Prices and codes can change, so confirm at checkout.

&copy; 2026 Sid Yadav
