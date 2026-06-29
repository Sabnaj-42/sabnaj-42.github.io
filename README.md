# sabnaj-42.github.io

Personal academic website for **Sabnaj Akter** — Distributed Systems Engineer & Researcher.
Live at **https://sabnaj-42.github.io**.

Hand-built static site: plain HTML + CSS + a little vanilla JS. No framework, no build step.

## Structure

```
index.html              # all content + sections
assets/
  css/style.css         # styling, light/dark themes, responsive
  js/main.js            # scroll-spy nav, reveal-on-scroll, theme toggle
  img/favicon.svg       # initials monogram favicon
  img/profile.jpg       # headshot (add this — see below)
  Sabnaj_Akter_CV.pdf   # downloadable CV
```

## Add your photo

Drop a square-ish headshot at `assets/img/profile.jpg`. Until it exists, the site shows an
"SA" monogram automatically — nothing breaks. ~600×600 px JPG is plenty.

## Edit content

Everything is plain text in `index.html`, grouped by clearly commented sections
(`<!-- ===== PROJECTS ===== -->`, etc.). Change the text, save, refresh.

## Preview locally

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy

This repo is a GitHub **user site**, so pushing to the `main` branch publishes automatically —
no Actions or Jekyll config needed.

```bash
git add -A
git commit -m "Update site"
git push
```

Live within ~1 minute at https://sabnaj-42.github.io
(Repo → Settings → Pages: Source = "Deploy from a branch", `main` / root.)
