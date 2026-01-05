# ATOM.css

**Tiny • dark • precise • interactive • configurable**

A minimal, modern, single-file CSS framework inspired by GitHub's dark theme. Perfect for documentation sites, personal pages, code-heavy blogs, or any project that needs a clean, professional dark (or light) look — without bloat.

- **~8 KB** minified
- No JavaScript required for most features
- CSS-only interactive components (tabs, accordions, tooltips)
- Built-in syntax highlighting via Highlight.js
- Optional configuration via `atcss.config.json`
- Theme support (dark/light/custom)
- Responsive sidebar, cards, alerts, improved form elements, and more

## Version

As of `5/1/2026`, _Atom.css_ is version `0.1`

## Demo

Open `tests/test.html` in your browser to see all features in action.

## Quick Start

1. Create a new HTML file:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Site – ATOM.css</title>

    <!-- Syntax Highlighting (recommended) -->
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.10.0/styles/github-dark.min.css"
    />
    <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.10.0/highlight.min.js"></script>

    <!-- Include CSS -->
    <link rel="stylesheet" href="atom.css" />
  </head>
  <body>
    <h1>Hello ATOM.css</h1>
    <p class="text-muted">Tiny, dark, and precise.</p>
  </body>
</html>
```

2. Add the JavaScript include at the bottom (before `</body>`) for copy buttons, modals, config loading, and syntax highlighting:

```html
<script src="atom.js"></script>
<script>
  hljs.highlightAll();
</script>
```

That's it — you're ready to go!

## Features

### Layout & Utilities

- Flexbox helpers: `.flex`, `.row`, `.col`, `.gap-1` to `.gap-5`, alignment, justification
- Spacing: `.p-`, `.px-`, `.py-`, `.m-` utilities
- Backgrounds, text colors, radius, shadows

### Components

- Buttons (`.btn`, colored variants)
- Labels / Tags
- Code blocks with **copy button** and **syntax highlighting**
- **Tabs/Pages** (pure CSS switching)
- Accordion (pure CSS)
- Tooltip
- Modal (JS toggle)
- Sidebar (fixed, mobile-friendly toggle)
- Cards with hover shadow
- Alerts (info, success, warning, danger)
- Progress bars
- Improved `<textarea>`

### Typography

- Clean headings and paragraph spacing
- Custom list styles (`.list-circle`, `.list-square`, `.list-none`)
- Inline code styling

### Configuration (Optional)

Create `atcss.config.json` in your project root:

```json
{
  "theme": "dark", // "dark" | "light" | custom via overrides
  "fonts": {
    "body": "Inter, system-ui, sans-serif",
    "headings": "Georgia, serif",
    "code": "Fira Code, monospace"
  },
  "custom": {
    ".sidebar a": {
      "color": "#58a6ff",
      "text-decoration": "none"
    },
    ".card": {
      "border": "1px solid #30363d"
    }
  },
  "overrides": {
    "--blue": "#79c0ff",
    "--radius-md": "12px"
  }
}
```

The framework automatically loads and applies this config on page load.

## Customization

All colors, spacing, and radii are CSS variables in `:root`. Override them directly or via the config file.

Light theme is built-in — just set `"theme": "light"` or add `data-theme="light"` to `<html>`.

## License

MIT 2026

Feel free to use, modify, and share.

---

Made with precision — for builders who value clarity.
