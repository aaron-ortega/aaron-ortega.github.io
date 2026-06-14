# resume-website

Single-page personal site with plain HTML/CSS/JS, no build step, ready for GitHub Pages.

## Structure

```
index.html              # the page (markup + small inline script)
assets/
  css/style.css         # styling (dark editorial theme, responsive)
  img/profile.jpg       # portrait
  resume.pdf            # downloadable resume (synced from ../resume/output/resume-_main.pdf)
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
