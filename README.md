# HTML Tools

Single-file HTML tools hosted on GitHub Pages. No build step, no frameworks, and no local installs required.

## Structure

- `index.html` - directory of tools (GitHub Pages entry point).
- `tools/` - each tool is a single `.html` file.
- `assets/` - shared icons and screenshots.
- `docs/` - optional developer notes.

## Add a tool

1. Copy `tools/_template.html` to `tools/<tool-name>.html` (use kebab-case).
2. Update the title, description, and footer links.
3. Implement the tool logic with inline CSS and JS.
4. Add the tool to `index.html`.
5. Commit and push. GitHub Pages serves it from the repo root.

## GitHub Pages

In GitHub: Settings -> Pages -> Deploy from a branch -> `main` (root).
Your site will be available at `https://tarazevits.io/tools/`.

## Conventions

- One HTML file per tool in `tools/`.
- Inline CSS and JS only.
- Dependencies via pinned CDN URLs (include versions).
- Mobile-friendly layouts, clear errors, and copy-to-clipboard for outputs.
- Add transcript or prompt links to the footer when available.

## Commands

There are no build, test, or lint commands yet.

For local previews, start a web server from the repo root (for example, `python -m http.server 8000`)
and open pages with the correct path, such as `http://localhost:8000/` or
`http://localhost:8000/tools/<tool-name>.html`.

## Included tools

- `tools/json-to-yaml.html` - Convert JSON into YAML.
