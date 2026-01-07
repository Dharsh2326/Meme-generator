# Meme Generator 

A lightweight React + Vite project that fetches meme templates from the Imgflip API and allows users to generate custom memes by editing the top/bottom text and picking a random image.

##  Features

- React components for Header and Main UI
- Fetches meme templates from `https://api.imgflip.com/get_memes`
- Controlled inputs for top/bottom text
- Button to pick a random meme image
- Vite for fast development and build
- ESLint configuration included

##  Quick Start

Install and run the dev server:

```sh
npm install
npm run dev
```

Build for production:

```sh
npm run build
```

Run ESLint:

```sh
npm run lint
```

Preview the production build:

```sh
npm run preview
```

## Project structure

- [index.html](index.html) — HTML entry that loads [index.jsx](index.jsx).
- [index.jsx](index.jsx) — Root entry that mounts the app (`createRoot` → [`App`](App.jsx)).
- [App.jsx](App.jsx) — Root app component (imports and renders [`Header`](components/Header.jsx) and [`Main`](components/Main.jsx)).
- [components/Header.jsx](components/Header.jsx) — Header component (shows logo at [images/troll-face.png](images/troll-face.png)).
- [components/Main.jsx](components/Main.jsx) — Main meme UI and logic (state for meme, fetches memes, and provides [`getMemeImage`](components/Main.jsx) and [`handleChange`](components/Main.jsx)).
- [index.css](index.css) — Global styles used by the root app (forms, meme layout).
- [vite.config.js](vite.config.js) — Vite configuration (React plugin).
- [package.json](package.json) — Scripts and dependencies.
- [eslint.config.js](eslint.config.js) — ESLint setup and rules.
- [.gitignore](.gitignore) — Ignored files for Git.

Additional files in `src/` (also included in the workspace):
- [src/main.jsx](src/main.jsx) — alternative entry (creates root and renders [`src/App.jsx`](src/App.jsx))
- [src/App.jsx](src/App.jsx) — app in `src/` (note: workspace contains both root `App.jsx` and `src/App.jsx`)
- [src/index.css](src/index.css) — theme styles used by `src/` app
- [src/App.css](src/App.css) — additional styles
- [src/assets/](src/assets/) — assets folder (empty/present)

Directories:
- [components/Header.jsx](components/Header.jsx)
- [components/Main.jsx](components/Main.jsx)
- [images/](images/) — contains [images/troll-face.png](images/troll-face.png)
- [public/](public/) — public assets

## 📌 Notes

This project was created as part of my React learning journey and helped me practice managing component state, handling user input, and integrating a public API for dynamic content.
