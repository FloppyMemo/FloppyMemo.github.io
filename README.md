# Caio Rocha, Cybersecurity Portfolio

Personal portfolio site focused on security operations and compliance. Built as a single self-contained HTML file, ready for GitHub Pages.

**Live site:** https://floppymemo.github.io

## Features

- **Bilingual (EN/PT):** opens in English by default, with an EN/PT toggle in the top bar. The visitor's choice is remembered in their browser.
- **Single file:** all HTML, CSS, and JavaScript live in `index.html`. No build step, no dependencies beyond Google Fonts.
- **Verifiable credentials:** certification cards link directly to Credly and Coursera verification pages.
- **Sections:** About, Experience, Education, Certifications, Skills, Hands-On Labs, and Contact.

## Publishing on GitHub Pages

1. Create a repository named `<your-username>.github.io` (this repo).
2. Push `index.html` and this `README.md` to the `main` branch:

   ```bash
   git init
   git add .
   git commit -m "portfolio: initial release"
   git branch -M main
   git remote add origin https://github.com/FloppyMemo/FloppyMemo.github.io.git
   git push -u origin main
   ```

3. On GitHub, go to **Settings → Pages**.
4. Under **Source**, select the `main` branch and the `/ (root)` folder. Save.
5. Wait 1 to 2 minutes. The site goes live at `https://<your-username>.github.io`.

## Editing content

All visible text lives in two places inside `index.html`:

- The HTML body (English defaults)
- The `translations` object inside the `<script>` tag at the bottom (EN and PT strings, keyed by the `data-i18n` attribute on each element)

To change any text, update both the HTML default and the matching key in `translations`. To add a new translatable element, give it a `data-i18n="your_key"` attribute and add the key with `en` and `pt` values to the object.

## Testing locally

Open `index.html` directly in a browser. No server needed.

## Structure

```
.
├── index.html   # complete site (HTML + CSS + JS in one file)
└── README.md    # this guide
```
