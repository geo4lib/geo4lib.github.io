# geo4lib.github.io

Zensical website for the Geo4Lib community.

The site keeps its existing `mkdocs.yml` configuration. Zensical supports this
format as its recommended migration path for existing Material for MkDocs
projects.

Zensical does not yet implement Material for MkDocs' blog plugin. Blog posts
remain in `docs/blog/posts/`, while `docs/blog/index.md` contains a
newest-first index that must be updated when a post is added.

## Local development

The site uses Python 3.12 and `uv`. From the repository root, create the
environment from the committed lockfile:

```bash
uv sync --locked
```

Start the development server:

```bash
uv run --locked zensical serve
```

Open <http://127.0.0.1:8000/>. The server automatically reloads after changes
to `mkdocs.yml` or files under `docs/`.

Before committing, run a strict production build:

```bash
uv run --locked zensical build --clean --strict
```

The generated `site/` directory is ignored. Pushes to `main` deploy the site to
GitHub Pages through `.github/workflows/publish.yml`. The repository's GitHub
Pages source must be set to **GitHub Actions**.
