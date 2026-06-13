# resume-website

Single-page personal site for Aaron Ortega — a gateway to socials and a place to
view/download the resume. Plain HTML/CSS, no build step, ready for GitHub Pages.

## Structure

```
index.html    # the page (hero + social links + inline resume)
style.css     # styling (dark/light theme, responsive)
resume.pdf    # downloadable resume (synced from ../resume/output/resume-_main.pdf)
```

## Local preview

```bash
open index.html          # or:
python3 -m http.server    # then visit http://localhost:8000
```

## Deploy (GitHub Pages)

Repo must be **public** for free GitHub Pages. Once public:
Settings → Pages → Source: `Deploy from a branch` → `main` / `root`.

## Updating the resume PDF

```bash
cp ../resume/output/resume-_main.pdf resume.pdf
```
