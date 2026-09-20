# DLX HTML CSS Starter

A lightweight starter template for vanilla HTML, CSS and JavaScript projects.

Built with a simple CSS architecture, design tokens, reusable utilities, local fonts and development rules for Cursor.

## Structure

```text
dlx-html-css-starter/
├── .cursor/
│   └── rules/
│       └── dlx-frontend.mdc
│
├── assets/
│   ├── fonts/
│   │   ├── roboto/
│   │   └── roboto-mono/
│   └── images/
│
├── css/
│   ├── reset.css
│   ├── fonts.css
│   ├── tokens.css
│   ├── global.css
│   ├── utilities.css
│   ├── welcome.css
│   └── style.css
│
├── js/
│   └── main.js
│
├── index.html
├── .gitignore
└── README.md
```

## CSS Architecture

The stylesheet structure separates global foundations from project-specific code.

- `reset.css` — browser normalization and sensible defaults
- `fonts.css` — local font declarations
- `tokens.css` — design tokens and reusable CSS custom properties
- `global.css` — global element styles
- `utilities.css` — reusable utility classes
- `welcome.css` — temporary DLX starter screen
- `style.css` — CSS entry point and project-specific styles

The stylesheets are imported through `style.css`:

```css
@import "./reset.css";
@import "./fonts.css";
@import "./tokens.css";
@import "./global.css";
@import "./utilities.css";
@import "./welcome.css";
```

## Welcome Screen

The starter includes a small DLX welcome screen that acts as a visual smoke test.

If the screen renders correctly, the HTML structure, CSS imports and local fonts are working.

When starting a real project:

1. Remove the welcome markup from `index.html`.
2. Remove the `welcome.css` import from `style.css`.
3. Delete `welcome.css`.
4. Start building your project.

The welcome styles are intentionally isolated so the DLX visual identity does not affect project styles.

## Local Fonts

The welcome screen uses local variable fonts:

- Roboto
- Roboto Mono

Font declarations are kept in:

```text
css/fonts.css
```

Font files are stored in:

```text
assets/fonts/
```

The DLX welcome screen uses Roboto for its primary typography and Roboto Mono for technical labels and interface details.

Project typography remains configurable through `tokens.css`.

## Cursor Rules

The project includes development guidelines for Cursor in:

```text
.cursor/rules/dlx-frontend.mdc
```

These rules define conventions for:

- semantic HTML
- BEM naming
- design tokens
- accessibility
- CSS architecture
- responsive layouts
- vanilla JavaScript
- minimal and focused code changes

## Usage

1. Create a new repository from this template.
2. Open `index.html` and confirm the DLX welcome screen is working.
3. Remove the welcome screen and its stylesheet.
4. Update the design tokens in `tokens.css`.
5. Add project assets to `assets/`.
6. Write project-specific styles in `style.css`.
7. Build.

## Principles

- Semantic HTML
- BEM naming
- Design tokens
- Responsive layouts
- Accessibility
- Minimal dependencies
- Simple, maintainable code

---

Built by **DLX**.
