# Theme Switcher with CSS Variables

A pure HTML + CSS theme switcher — no JavaScript — built to showcase a
scalable design-token architecture. Three complete themes (**Light**,
**Dark**, and **Aurora**, a glassmorphic/neon variant) share one set of
semantic CSS custom properties, and switching between them is handled
entirely with radio inputs, `:checked`, and the `:has()` selector.

## Live Project Page

`https://<your-username>.github.io/<repo-name>/`
*(replace with your deployed URL after enabling GitHub Pages — see below)*

## Features

- **Zero JavaScript theming** — driven by `<input type="radio">`,
  `<label>`, `:checked`, and `:has()`.
- **Single token system** — `--color-bg`, `--color-surface`, `--color-text`,
  `--shadow-*`, `--radius-*`, `--spacing-*`, `--transition-*`, etc., all
  redefined per theme at the `:root` / `html` level. No component ever
  hardcodes a color.
- **Animated switcher** — a sliding pill indicator tracks the active theme.
- **Aurora theme** — glassmorphism, layered gradients, and soft glow shadows.
- **Accessible by default** — semantic `<fieldset>`/`<legend>`, proper
  label association, visible focus rings, keyboard-only operability.
- **Responsive** — tuned breakpoints for desktop, tablet, and mobile.
- **Respects `prefers-reduced-motion`.**

## Project Structure

```
.
├── index.html   # Semantic markup: theme inputs, switcher, preview card
├── style.css    # Reset, design tokens, themes, layout, components
└── README.md
```

## Running Locally

No build tools or dependencies required.

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

Then either open `index.html` directly in a browser, or serve it:

```bash
python3 -m http.server 8000
# visit http://localhost:8000
```

## Deploying with GitHub Pages

1. Push your code to the `main` branch.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set Source to **Deploy from a branch**,
   branch `main`, folder `/ (root)`.
4. Save. Your site goes live at
   `https://<your-username>.github.io/<repo-name>/` within a minute or two.

## Browser Support

Theme switching relies on the CSS `:has()` selector, supported in current
versions of Chrome, Edge, Safari, and Firefox 121+.

## License

MIT
