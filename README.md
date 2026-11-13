# 21 Days, 21 Projects

Twenty-one small web projects, built one a day. Every project is a **single HTML file**
that holds its own CSS and JavaScript. No build step, no install, no npm, no CDN, no
account, no server. Double-click a file and it runs.

**[Open the dashboard &rarr;](index.html)**

**Live:** https://neharajput0502.github.io/21-day-build-lab/

## Add your own project

This lab is open source and open to contributions. Build something useful or fun in a single HTML
file, send a pull request, and it goes live here with your name on it. Start with the
[contributing guide](CONTRIBUTING.md) and the [project template](community/TEMPLATE.html).

---

## How it fits together

    index.html                     the dashboard: all 21 days
    projects/day-01-moving-heart/index.html
    projects/day-02-neon-name/index.html
    projects/day-03-birthday-wish/index.html
    ...
    projects/day-20-catch-the-dot/index.html
    projects/day-21-portfolio-generator/index.html
    community/<username>/<project>/index.html   projects added by contributors

The dashboard links to all 21 projects. Every project links back to the dashboard and
sideways to the day before and the day after, so you can walk the whole series without
returning to the index.

Inside any project:

| Key | What it does |
| --- | --- |
| <kbd>&larr;</kbd> | Previous day |
| <kbd>&rarr;</kbd> | Next day |
| <kbd>Esc</kbd> | Back to the dashboard |

The dashboard remembers which days you have opened, in your own browser only. Clear it
any time with the link under the day strip.

---

## The 21 projects

&#11088; marks the five with the strongest reaction from viewers.

| Day | Project | Input &rarr; output | Comment keyword |
| ---: | --- | --- | --- |
| 01 | [Moving Heart](projects/day-01-moving-heart/index.html) | A name &rarr; Animated beating heart | `HEART` |
| 02 | [Neon Name Generator](projects/day-02-neon-name/index.html) | Name and colour &rarr; Glowing neon sign | `NEON` |
| 03 | [Birthday Wish Maker](projects/day-03-birthday-wish/index.html) | A name &rarr; Cake, balloons, confetti | `BIRTHDAY` |
| 04 | [Love Message Generator](projects/day-04-love-message/index.html) | Two names &rarr; Romantic animation | `LOVE` |
| 05 | [Particle Text Animation](projects/day-05-particle-text/index.html) | Any text &rarr; Text assembled from particles | `PARTICLE` | ⭐
| 06 | [Cursor Galaxy](projects/day-06-cursor-galaxy/index.html) | Mouse movement &rarr; Stars trailing the cursor | `GALAXY` |
| 07 | [Liquid Button](projects/day-07-liquid-button/index.html) | One click &rarr; Liquid splash animation | `LIQUID` |
| 08 | [Password Strength Checker](projects/day-08-password-checker/index.html) | A password &rarr; Strength score and fixes | `PASSWORD` |
| 09 | [Gradient Generator](projects/day-09-gradient-generator/index.html) | Two colours &rarr; Live background plus CSS | `GRADIENT` |
| 10 | [Glassmorphism Generator](projects/day-10-glassmorphism/index.html) | Sliders &rarr; Glass UI plus CSS | `GLASS` |
| 11 | [Colour Palette Extractor](projects/day-11-color-palette/index.html) | A photo &rarr; Matching colour palette | `PALETTE` | ⭐
| 12 | [Image Filter Editor](projects/day-12-image-filter/index.html) | An image &rarr; Filtered, downloadable image | `FILTER` | ⭐
| 13 | [Image Compressor](projects/day-13-image-compressor/index.html) | An image &rarr; Smaller file, same photo | `COMPRESS` |
| 14 | [Digital Signature Pad](projects/day-14-signature-pad/index.html) | A drawn signature &rarr; Transparent PNG download | `SIGNATURE` |
| 15 | [QR Code Generator](projects/day-15-qr-generator/index.html) | Text or a link &rarr; Scannable QR code | `QR` | ⭐
| 16 | [Bill Splitter](projects/day-16-bill-splitter/index.html) | Bill and headcount &rarr; Amount per person | `SPLIT` |
| 17 | [EMI Calculator](projects/day-17-emi-calculator/index.html) | Loan details &rarr; Monthly EMI and schedule | `EMI` |
| 18 | [Typing Speed Test](projects/day-18-typing-speed/index.html) | Typed text &rarr; WPM and accuracy | `TYPING` |
| 19 | [Reaction-Time Game](projects/day-19-reaction-game/index.html) | Wait, then click &rarr; Reaction time in ms | `REACTION` |
| 20 | [Catch-the-Dot Game](projects/day-20-catch-the-dot/index.html) | Clicks on a moving dot &rarr; Score and timer | `GAME` |
| 21 | [Mini Portfolio Generator](projects/day-21-portfolio-generator/index.html) | Your details &rarr; A personal portfolio page | `PORTFOLIO` | ⭐

---

## Running it

**Locally.** Download or clone the repo and open `index.html` in Chrome, Edge, Firefox
or Safari. Keep `index.html` and the `projects/` folder together.

**On the web.** Push the repo to GitHub, then Settings &rarr; Pages &rarr; Deploy from
branch &rarr; `main` / `/ (root)`. Your dashboard lands at
`https://<your-username>.github.io/21-day-build-lab/` and each project sits at a clean
URL like `/projects/day-15-qr-generator/`. That is the link to put in your Instagram bio.

`.nojekyll` is included so GitHub Pages serves the folders untouched.

---

## What runs where

Everything runs in your browser. Images you upload, passwords you type, signatures you
draw and numbers you enter are never sent anywhere, because there is nothing to send them
to. Downloads are produced by the browser itself.

A few honest limits:

- The password checker is a teaching tool that estimates patterns. It does not check
  breach databases.
- The EMI calculator assumes a fixed annual rate on a monthly reducing balance, and
  ignores fees and insurance. Your lender's schedule may differ.
- Game timings include browser and device latency, so treat them as casual scores.
- Image tools accept files up to 30&nbsp;MB and cap processing at 2200&nbsp;px on the
  longest side. Animated GIFs are read as still images.
- Decorative animation respects `prefers-reduced-motion`.

---

## Making it yours

Open any project in a text editor. The CSS sits in one `<style>` block and the JavaScript
in one `<script>` block at the bottom, so there is nothing to hunt for. Sample names,
colours and links are placeholders; replace them.

If you rename a project folder, update the matching link in `index.html` and the
prev/next links in its two neighbours.

## Credits

The QR encoder embeds [Project Nayuki's QR Code generator library](https://www.nayuki.io/page/qr-code-generator-library)
under the MIT licence. See `THIRD-PARTY-NOTICES.md`. Everything else was written for this
collection.
