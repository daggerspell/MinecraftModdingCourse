# NeoForge 1.21.1 Modding Course — Site

This repo contains a MkDocs Material site for the course.

## Quickstart

1) Install Python 3.9+.
2) Install dependencies:
   - Windows: `py -m pip install -r requirements.txt`
   - macOS/Linux: `python3 -m pip install -r requirements.txt`
3) Run local preview: `mkdocs serve` then open http://127.0.0.1:8000
4) Build static site: `mkdocs build` (outputs to `site/`).

## GitHub Pages

- The workflow `.github/workflows/gh-pages.yml` is manual (`workflow_dispatch`).
- When you’re ready to publish, run it from the Actions tab.
- Before publishing, set `site_url`, `repo_url`, and `repo_name` in `mkdocs.yml`.

## Content

- Write pages in `docs/` as Markdown (Material supports rich features).
- Start with `docs/syllabus.md` by converting the provided DOCX.

## Converting the syllabus (optional)

If you have Pandoc installed:

```bash
pandoc -s "NeoForge_1.21.1_Modding_Course_Syllabus_and_Outline.docx" -t gfm -o docs/syllabus.md
```

Then tidy headings and add frontmatter as needed.
