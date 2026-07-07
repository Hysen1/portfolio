# Portfolio — Hysen

A single-page portfolio combining web development / SEO work and journalism work (Mediaplus, Apollon).

No build step — it's one static `index.html` plus two images. That makes it a good fit for **GitHub Pages**, which is free and easily handles 1–2 visitors a day.

## Structure

```
portfolio/
├── index.html          ← the whole site
└── assets/
    ├── city-center-1.png
    └── city-center-2.png
```

## Publish it on GitHub Pages (5 minutes)

1. Create a new repository on GitHub (e.g. `portfolio`), keep it **public** — GitHub Pages needs public repos on the free plan.
2. From inside this `portfolio` folder, run:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/<your-username>/portfolio.git
   git push -u origin main
   ```
3. On GitHub: go to the repo → **Settings → Pages** → under "Build and deployment", set **Source: Deploy from a branch**, branch `main`, folder `/ (root)` → **Save**.
4. GitHub gives you a URL within a minute or two, usually:
   `https://<your-username>.github.io/portfolio/`
5. (Optional) Add a `CNAME` file with a custom domain if you want to serve it from your own domain instead.

## Editing content later

Everything lives in `index.html` — project cards are under `<section id="builds">`, journalism under `<section id="dispatches">`. Duplicate a `<article class="card">` block to add a new site, or a `<div class="dispatch">` block to add a new outlet.

## Things to double-check before sending to clients

- Swap the placeholder contact email (`hello@fotnet24.net`) for the address you actually want clients to use.
- The three Apollon YouTube embeds and the Mediaplus Dailymotion link are pulled straight from the URLs you gave me — worth a quick click-through to confirm they're the segments you want featured.
- The City Center screenshots are embedded directly (domain has expired, so there's no live link to send people to).
