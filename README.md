# J&B Furniture Liquidation and Filipino/Asian Store — Website

A single-file website for J&B Store at 5645 Ferry St., Niagara Falls, ON.  
Built to drive foot traffic to the physical store — no online shop or checkout.

---

## Files

```
jb_store_website.html   — The entire website (one file, no dependencies)
README.md               — This file
```

---

## How to Open Locally

Double-click `jb_store_website.html` — it opens in any browser. No installation needed.

---

## How to Publish Online

**Option A — Netlify (free, easiest)**
1. Go to https://netlify.com and create a free account
2. Drag and drop `jb_store_website.html` onto the Netlify dashboard
3. Your site is live instantly at a `.netlify.app` URL
4. Optional: connect a custom domain (e.g. `jbstore.ca`)

**Option B — GitHub Pages (free)**
1. Create a GitHub account at https://github.com
2. Create a new repository named `jb-store`
3. Upload `jb_store_website.html` and rename it `index.html`
4. Go to Settings → Pages → set source to `main` branch
5. Site goes live at `https://yourusername.github.io/jb-store`

**Option C — Existing hosting (GoDaddy, Bluehost, etc.)**
1. Log into your hosting control panel
2. Open File Manager and navigate to `public_html`
3. Upload `jb_store_website.html` and rename it `index.html`

---

## How to Edit Content

Open `jb_store_website.html` in any text editor (Notepad, VS Code, TextEdit).

| What to change | Where to find it |
|---|---|
| Phone numbers | `<div class="topbar">` near the top |
| Address & hours | Same `topbar` section |
| Hero tagline | `<h1>` inside `<section class="hero">` |
| Department names | `<div class="cat-card">` blocks |
| About text | `<div class="about-left">` section |
| Footer links | `<footer>` at the bottom |

---

## How to Change Colors

At the top of the HTML file, inside `<style>`, find the `:root` block:

```css
:root {
  --copper: #B87333;       /* Main accent color */
  --black: #0A0704;        /* Background */
  --warm-white: #F9F4EE;   /* Text color */
  --mid: #8C7B6B;          /* Muted text */
}
```

Change `--copper` to any hex color and the entire site updates.

---

## How to Add Photos

The department cards currently show placeholder text. To add a real photo to a card, find a `.cat-card` block and add a background image:

```html
<div class="cat-card" style="background-image: url('your-photo.jpg'); background-size: cover;">
```

Place your photos in the same folder as the HTML file and reference them by filename.

---

## Store Information

| | |
|---|---|
| Owner | John & Beth Wright |
| Address | 5645 Ferry St., Niagara Falls, ON L2G 1S5 |
| Tel | 289-296-1114 |
| Cell | 905-371-6600 / 905-324-5077 |

---

## Notes

- The site uses Google Fonts (Cormorant Garamond + Jost). An internet connection is required to load them. For fully offline use, the fonts can be downloaded and hosted locally.
- No cookies, tracking, or third-party scripts are included.
- The Ria Remittance and Get Directions buttons link to Google Maps and `tel:` links — these work automatically on phones.
