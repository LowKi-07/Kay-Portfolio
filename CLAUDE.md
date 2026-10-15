# CLAUDE.md

Personal portfolio for Kishore S, served at kishoresv.com via GitHub Pages (`CNAME`) from `main`.

## Structure

- `index.html` — the whole site: inline CSS and JS, no build step. Pages (Home, Work, Case Study, About me) are `<main class="page">` sections switched by `data-page` links.
- `Assets/logos/` — "Worked With" brand logos, rendered monochrome via CSS filters.
- `Assets/projects/` — project thumbnails for the home and Work pages.
- `resume/resume.html` — source for `Assets/Kishore-S-Resume.pdf`.

## Commands

```bash
# Preview locally at http://localhost:8080
python3 -m http.server 8080

# Regenerate the resume PDF after editing resume/resume.html (must stay one A4 page)
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new --no-pdf-header-footer --virtual-time-budget=8000 --print-to-pdf=Assets/Kishore-S-Resume.pdf "file://$PWD/resume/resume.html"
```
