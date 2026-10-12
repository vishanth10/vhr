# vishanth.me

Personal site of Vishanth Hari Raj Balasubramanian, built with **Jekyll 4** and deployed to GitHub Pages by GitHub Actions (`.github/workflows/pages.yml`).

## Editing content
Almost everything lives in `_data/`, so you rarely need to touch HTML:

| File | What it holds |
|---|---|
| `_data/experience.yml` | Companies, roles, dates, highlights (supports **bold** and [links]()) |
| `_data/projects.yml` | Project cards; `category` is `llm`, `dl` or `oss` |
| `_data/skills.yml` | Skill groups |
| `_data/education.yml` | Degrees |
| `_data/honors.yml` | Certifications, awards, languages |
| `_data/stats.yml` | The four headline numbers |

The page layout is `index.html`; styles are in `assets/css/style.css`; interactions in `assets/js/main.js`.

## Résumé
The PDF is `assets/Vishanth_HariRaj_Resume.pdf`. Its source is `_resume/resume.html` (not published). To regenerate it, print that file to PDF with Chrome (Letter, no headers/footers).

## Analytics
Set `analytics.google_id` (GA4) and/or `analytics.goatcounter` in `_config.yml`. Scripts load only on the live site.

## Run locally
```sh
bundle install
bundle exec jekyll serve --livereload   # http://localhost:4000
```
