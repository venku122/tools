# Repository Guidelines

## Project Structure & Module Organization

- `index.html` - directory of tools (GitHub Pages entry point).
- `tools/` - single-file HTML tools.
- `tools/_template.html` - starting point for new tools.
- `assets/` - shared icons, screenshots.
- `docs/` - optional developer notes.
- `scripts/` - optional maintenance scripts.

## Tool Constraints

- One HTML file per tool in `tools/`.
- Inline CSS and JS only.
- No build step and no frameworks like React.
- Dependencies only via pinned CDN URLs (include versions).
- Keep tools self-contained and copy-paste friendly.

## UX Requirements

- Mobile-friendly layouts with large tap targets.
- Provide copy-to-clipboard for outputs.
- Clear error states and status messaging.
- Respect `prefers-reduced-motion`.

## Security & Data Handling

- Never commit secrets.
- If a tool needs an API key, prompt the user and store it in `localStorage` (never in query params).
- Keep user data in the browser unless they opt in to sharing it.

## Documentation

- Each tool must include a title and purpose at the top of the HTML file.
- Footers must include "View source" and "Transcript" links (placeholders are OK until you have the real URLs).
- Update `index.html` with title, description, and link for each new tool.
- PR descriptions should mention transcript or prompt links when available.

## Build, Test, and Development Commands

- None yet. Document new commands here and in `README.md` if added.

## Coding Style & Naming Conventions

- Indentation: 2 spaces for HTML, CSS, and JS.
- Filenames: kebab-case for tools and directories.
- Use a formatter if one is introduced.

## Testing Guidelines

- No testing framework yet. If added, use `tests/` with clear naming.

## Commit & Pull Request Guidelines

- Use clear, imperative commit messages (or Conventional Commits).
- PRs include a summary, testing notes, and transcript or prompt links when available.
