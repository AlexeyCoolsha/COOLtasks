# COOLtasks

A Vite-powered front-end sandbox for static pages, styling experiments, and UI components. The project is structured for multi-page HTML development with Sass, so you can build and preview several pages in a single Vite build.

## ✨ Highlights

- **Vite + ES modules** for fast local development.
- **Multi-page build**: any `*.html` file in the repo becomes a build entry.
- **Sass architecture** with organized layers for base, components, layout, themes, and vendors.

## 🧩 Project Structure

```
.
├── src/
│   ├── html/pages/          # HTML pages (multi-page build entries)
│   ├── styles/              # Sass architecture
│   └── main.js              # Entry point that imports main.scss
├── public/                  # Static public assets
└── vite.config.js           # Multi-page Vite config
```

## 🚀 Getting Started

1. Install dependencies:

```bash
npm install
```

2. Start the dev server:

```bash
npm run dev
```

3. Build for production:

```bash
npm run build
```

4. Preview the production build:

```bash
npm run preview
```

## 🛠 How the Multi-Page Build Works

The Vite config automatically discovers **all** `*.html` files in the repository (excluding `node_modules` and `dist`). Each HTML file becomes an entry point in the build output, enabling multi-page sites without extra config.

## 🎨 Styling Notes

- The main stylesheet lives at `src/styles/main.scss` and is imported in `src/main.js`.
- Styles are organized by layers: **abstracts**, **base**, **components**, **layout**, **pages**, **themes**, and **vendors**.

---

If you'd like new pages, components, or a design system layer, feel free to extend the `src/html` and `src/styles` directories.
