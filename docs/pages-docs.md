# Pages and Documentation

This template uses MkDocs Material and GitHub Pages.

## Local Preview

```bash
python -m pip install -r requirements-docs.txt
mkdocs serve
```

## Strict Build

```bash
mkdocs build --strict
```

## GitHub Pages Setup

1. Open repository settings.
2. Go to Pages.
3. Set source to GitHub Actions.
4. Run the Pages workflow.

## Child Repository Updates

When creating a child repository, update:

- `site_name`
- `site_description`
- `site_url`
- `repo_url`
- navigation entries
