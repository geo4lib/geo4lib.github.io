# geo4lib.github.io

Material for MkDocs website for the Geo4Lib community.

## Local development

The site uses Python 3.12 and `uv`. From the repository root, create the
environment from the committed lockfile:

```bash
uv sync --locked
```

Start the development server:

```bash
uv run --locked mkdocs serve
```

Open <http://127.0.0.1:8000/>. The server automatically reloads after changes
to `mkdocs.yml` or files under `docs/`.

Before committing, run a strict production build:

```bash
uv run --locked mkdocs build --strict
```

The generated `site/` directory is ignored. Pushes to `main` deploy the site to
GitHub Pages through `.github/workflows/publish.yml`.
