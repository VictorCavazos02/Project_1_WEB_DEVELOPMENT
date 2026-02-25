# AI Assistant Instructions for Project_1_WEB_DEVELOPMENT

This repository is a very small static web page called **TweeterPage**. The codebase consists of a single HTML file (`index.html`), a CSS stylesheet (`external_style_sheets.css`), and an `images/` directory containing assets. There is no JavaScript, build system, package manager, or automated tests. The only project workflow is opening `index.html` in a browser to view changes.

## Project Structure and Purpose

- `index.html` – the entire page markup. It uses semantic HTML with a header section and a simple tweet input area.
- `external_style_sheets.css` – global stylesheet. All styling is done here with class selectors. Currently it sets background colors, layout with flexbox, and simple dimensions.
- `images/` – holds static assets (Twitter symbol, profile picture, etc.). When adding images, use relative paths like `./images/you.png`.

This is not a multi‑page or dynamic application; it was written as an exercise or prototype for a mock Twitter interface.

## Key Conventions

- **Class names** are lowercase with underscores or hyphens (`.centered_header`, `.tweet_table`, `.profile_pic`, `.sample_text`). When extending styles, follow the same simple naming.
- The stylesheet is linked directly from the `<head>` of `index.html` via `<link rel="stylesheet" href="external_style_sheets.css">`.
- Colors are often hardcoded (`ghostwhite`, `white`, `#1EA1FF` for the header text).
- Layout uses flex container for the header and percentage widths for the tweet box. Keep proportions similar when adding new components.
- No JavaScript means any interactive behavior should be simulated or described; avoid suggesting frameworks or build tooling unless explicitly requested by a user.

## Developer Workflow Notes

- There is **no build or test pipeline**. Editing the HTML/CSS and refreshing the browser is the usual process.
- To preview changes, open `index.html` in a local browser (e.g. `file:///` path or a simple static server).
- If new assets are added (images, fonts), place them in the appropriate directory and adjust paths accordingly.
- Commit messages should reflect simple changes ("add tweet input styling", "update header color").

## Guidelines for AI Coding Agents

When making suggestions or changes:

1. **Stay within the static-site context.** Do not introduce unrelated technologies (React, build systems, server code) unless the user explicitly asks to transform the project.
2. **Preserve existing structure.** Add new classes to `external_style_sheets.css` and reference them in `index.html`. Maintain the layout pattern (header centered, body width ~40% with margin-left 30%).
3. **Keep styling simple.** The stylesheet currently uses plain selectors and inline values; continue that pattern rather than refactoring into advanced preprocessors.
4. **Assets go in `images/`.** When suggesting new images, reference them relatively and ensure they exist or mention the need to add them.
5. **No tests or build commands to suggest.** If a user asks about testing or building, explain that none exist and recommend simple manual verification.
6. **Read README.md** – it currently only states the project name and purpose; nothing else. If the README needs updates, you can suggest adding more descriptive text but keep it minimal.
7. **Be explicit about file names** when giving examples (e.g., modify `external_style_sheets.css`, open `index.html`).

## Example Tasks

- *Add a new tweet entry below the existing one:* modify the HTML to duplicate the `.tweet_table` block and perhaps adjust CSS for multiple entries.
- *Change colors or fonts:* edit `external_style_sheets.css` as needed; refer to existing declarations for pattern.
- *Introduce a new section (e.g., sidebar):* add markup in `index.html` and corresponding style rules.

> ⚠️ This project is intentionally minimal. Do not overengineer solutions or add unnecessary dependencies.

Feel free to ask follow‑up questions if any part of the structure or conventions is unclear.