# Conversion Landing Page Template

A professional, high-conversion landing page built with **HTML + CSS + Vanilla JavaScript** and ready for **GitHub Pages**.

## Project structure

```bash
.
├── index.html
├── assets
│   ├── css
│   │   └── style.css
│   ├── js
│   │   └── main.js
│   └── img
│       ├── author-photo.svg
│       ├── hero-mockup.svg
│       └── og-cover.svg
└── README.md
```

## How to customize text content

1. Open `index.html`.
2. Update section copy directly:
   - Hero: headline, subtitle, CTA labels
   - Problem, Solution, Benefits, Included
   - Testimonials, Author bio, Offer details
   - FAQ and Footer info
3. Keep semantic structure and heading hierarchy (`h1` once, then `h2`, `h3`).

## How to change colors

Open `assets/css/style.css` and edit the variables inside `:root`:

```css
:root {
  --color-primary: #162033;
  --color-secondary: #eff3fa;
  --color-accent: #d96f1d;
  --color-bg: #f8f9fc;
  --color-text: #1f2937;
  --color-muted: #5c6677;
}
```

> Keep `--color-accent` for CTA buttons to preserve conversion emphasis.

## How to update sections

- Each mandatory section has a dedicated `<section id="...">` block in `index.html`.
- To add/remove cards (benefits, testimonials, included), duplicate or remove `<article class="card">` blocks.
- FAQ accordion items are inside `.faq-list`.
- JavaScript behavior is in `assets/js/main.js`:
  - FAQ expand/collapse
  - Fade-in reveal on scroll

## Deploy to GitHub Pages

1. Push this project to a GitHub repository.
2. Go to **Repository Settings → Pages**.
3. Under **Build and deployment**, choose:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` (or your default branch), folder `/root`
4. Save and wait for deployment.
5. Your site will be available at:
   - `https://<your-username>.github.io/<repo-name>/`

## Local preview

Use any static server, for example:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.
