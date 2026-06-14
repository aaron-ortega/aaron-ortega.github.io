# resume-website

Single-page personal site — plain HTML and CSS with a small inline script, no build step, ready for GitHub Pages.

## Structure

```
index.html                    # the page (markup + small inline script)
assets/
  css/style.css               # styling (dark editorial theme, responsive)
  img/profile.jpg             # portrait
  icons/apple-touch-icon.png  # iOS home-screen icon
  ortega-resume-june2026.pdf  # downloadable resume
```

## Local preview

```bash
python3 -m http.server   # then visit http://localhost:8000
```

(Use a server rather than opening the file directly so relative asset paths resolve.)

## Formatting & linting

```bash
npm install        # one-time: installs prettier + stylelint
npm run format     # prettier --write .
npm run lint:css   # stylelint **/*.css
```

## Deploy (GitHub Pages)

Repo must be **public** for free GitHub Pages. Once public:
Settings → Pages → Source: `Deploy from a branch` → `main` / `root`.
