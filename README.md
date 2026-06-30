# Theme Switcher with CSS Variables

A pure HTML + CSS theme switcher — no JavaScript — built to showcase a scalable design-token architecture. Three complete themes (**Light**, **Dark**, and **Aurora**, a glassmorphic/neon variant) share one set of semantic CSS custom properties, and switching between them is handled entirely with radio inputs, `:checked`, and the `:has()` selector.

## Challenge

This project was built as part of the **roadmap.sh** frontend project series.

**Challenge URL:** https://roadmap.sh/projects/theme-switcher

## Live Demo

https://<your-username>.github.io/<repo-name>/

> Replace the placeholder with your GitHub Pages URL after deployment.

## Features

- **Zero JavaScript theming** — driven by `<input type="radio">`, `<label>`, `:checked`, and `:has()`.
- **Single token system** — `--color-bg`, `--color-surface`, `--color-text`, `--shadow-*`, `--radius-*`, `--spacing-*`, `--transition-*`, etc., all redefined per theme. No component ever hardcodes a color.
- **Animated switcher** — a sliding pill indicator tracks the active theme.
- **Aurora theme** — glassmorphism, layered gradients, and soft glow shadows.
- **Accessible by default** — semantic `<fieldset>`/`<legend>`, proper label association, visible focus rings, and keyboard-only operability.
- **Responsive** — optimized for desktop, tablet, and mobile devices.
- **Respects `prefers-reduced-motion`.**

## Project Structure

```text
.
├── index.html
├── style.css
└── README.md
```

## Running Locally

No build tools or dependencies are required.

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

Then either open `index.html` directly in your browser or serve it locally:

```bash
python3 -m http.server 8000
```

Visit:

```
http://localhost:8000
```

## Deployment

Deploy using **GitHub Pages**:

1. Push your project to the `main` branch.
2. Navigate to **Settings → Pages**.
3. Under **Build and deployment**, select:
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Save your changes.

Your website will be available at:

```
https://<your-username>.github.io/<repo-name>/
```

## Browser Support

Theme switching relies on the CSS `:has()` selector, which is supported in current versions of:

- Google Chrome
- Microsoft Edge
- Safari
- Firefox 121+

## Technologies Used

- HTML5
- CSS3
- CSS Custom Properties (Design Tokens)
- CSS `:has()` Selector
- Flexbox
- CSS Grid

## License

This project is licensed under the **MIT License**.
