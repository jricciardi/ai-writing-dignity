# AI Writing Dignity

An editorial-style site exploring how to use AI to become a better writer—guided by a skeptical, seasoned editor-in-chief perspective. Interactive glossary “hover” tooltips provide RPG-style context on key terms.

## Tech
- Vite + React + TypeScript
- MDX for interactive editorial content
- HashRouter for GitHub Pages-friendly routing
- Glossary hover tooltips for RPG-style “term popups”

## Local Development
```bash
npm install
npm run dev
```

## Build
```bash
npm run build
npm run preview
```

## Deploy to GitHub Pages
This repo includes a GitHub Actions workflow that builds and deploys on every push to `main`.

Steps:
1. Push to `main`.
2. In Settings → Pages, set Source to “GitHub Actions”.
3. The workflow will publish to GitHub Pages (environment: github-pages).

If you use a custom domain, configure it in Pages and add a `CNAME` file in `public/`.

## Content
- Add MDX articles in `src/content/articles`.
- Add glossary terms in `src/content/glossary.json`.
- Use `<GlossaryHover term="...">` inside MDX to add RPG-style hovers.
