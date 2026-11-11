# Project guidance

This repository is a GitHub Pages website built with Jekyll.

- Keep page content in the existing root-level `.html` files and preserve their current URLs unless a change explicitly requires otherwise.
- Use Jekyll front matter and the shared layout in `_layouts/` for page metadata and the document shell.
- Put reusable markup in `_includes/` and reference it with Liquid `{% include ... %}` tags.
- Keep shared styles in `styles.css`; use `relative_url` for asset URLs generated in layouts so the site works with GitHub Pages base paths.
