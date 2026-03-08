# Repository Overview
This workspace contains a very small static project used for practicing HTML and CSS while following the `Curso Gustavo Guanabara` lessons. At the moment the only two source files are:

- `praticar.html` – the HTML document
- `praticar.css` – the stylesheet

Both files are empty placeholders; the intent is to write sample markup and styles as you work through exercises.

---

## Architecture & Big Picture

There is no application architecture beyond a flat, static website. No build tools, package managers, servers, or frameworks are involved. The HTML file links to the CSS file directly:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Prática</title>
  <link rel="stylesheet" href="praticar.css">
</head>
<body>
  <!-- add your markup here -->
</body>
</html>
```

You are free to add additional files or folders if the lesson requires them, but nothing in the existing tree depends on anything else.

---

## Developer Workflows & Commands

There are no build or test commands.

1. Edit `praticar.html` and `praticar.css` in the editor.
2. Open `praticar.html` in a browser (double‑click from the file explorer or use Live Server extension) to see changes.
3. Save frequently; there is no watch/compile step.

Tips:
- Use the browser's devtools to inspect elements and experiment with CSS rules.
- If you install the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension, right‑click `praticar.html` and choose "Open with Live Server" for automatic reloads.

---

## Project‑Specific Conventions

- Class and id names may be in Portuguese to match the course examples (e.g. `.conteudo`, `#cabecalho`).
- Keep presentational styles in `praticar.css`; the HTML should be semantic.
- There is no JavaScript in this workspace unless a lesson adds it – if you do add `.js` files, simply include them with `<script>` tags.

---

## AI Agent Guidance

When an AI coding agent works in this repository it should:

1. Recognise that the codebase is a static HTML/CSS exercise space, not a full‑stack application.
2. Avoid introducing build tooling, dependencies, or folder structures that don't match the simple flat layout unless the user explicitly requests it.
3. Provide concrete, minimal examples inline. For instance, when asked to add a navigation bar, generate the `<nav>` markup and corresponding CSS rules inside `praticar.css`.
4. Keep comments and variable names in Portuguese if the prompt or surrounding context uses Portuguese.
5. Do not assume any testing framework; there is no `package.json` or `Makefile`.
6. When saving styles, reference the existing stylesheet path exactly (`praticar.css`).

---

## Integration & External Dependencies

None. This is purely client‑side code. External resources (fonts, CDNs) can be linked directly in the HTML if needed by an exercise.

---

If anything in these instructions is unclear or if you would like the agent to cover additional patterns that show up while you work, please let me know so I can iterate accordingly.