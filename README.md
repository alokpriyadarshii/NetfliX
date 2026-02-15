# NetfliX

A Netflix style **web UI clone** built with **Vue 3 + Vite + Tailwind CSS**.  
This is a **UI/learning project** (no real Netflix API/auth) — it uses **local posters + MP4 trailers** and a smooth carousel browsing experience.

---

## ✨ What’s inside
- Left sidebar navigation (icons + Netflix logo)
- Featured hero **autoplay looping video** with title, year, genres, description
- Multiple **movie rows** using `vue3-carousel`
- Click a poster to open **full-screen playback** (with controls + back button)
- Global state via **Pinia** (current movie + full screen toggle)
- Animations via `animate.css`

---

## 🚀 Quick Start (all commands at once)

~~~bash
set -euo pipefail
cd "/Users/alok/Desktop/NetfliX"
npm install
npm run dev
~~~

---

## 🧹 If build / install issues (optional)

~~~bash
set -euo pipefail
cd "/Users/alok/Desktop/NetfliX"
rm -rf node_modules
npm ci
npm run dev
~~~

---

## 📦 Production build (optional)

~~~bash
set -euo pipefail
cd "/Users/alok/Desktop/NetfliX"
npm run build
npm run preview
~~~

> Production output goes to `dist/`.

---

## 📁 Project structure (high level)

~~~text
NetfliX/
  public/
    images/            
    videos/              
    favicon.ico
  src/
    components/
      MovieDetails.vue
      VideoCarousel.vue
    stores/
      movie.js
    router/
      index.js
    assets/
      main.css
    movies.json         
    App.vue              
    main.js              
  index.html
  tailwind.config.js
  postcss.config.js
  vite.config.js
  package.json
  package-lock.json
~~~

---

## 🛠 Customize
- **Add / edit movies**: update `src/movies.json`
- **Posters**: put PNGs in `public/images/` named exactly like the movie `name` (example: `Aftersun.png`)
- **Videos**: put MP4s in `public/videos/` named exactly like the movie `name` (example: `Aftersun.mp4`)
- **Categories / rows**: edit the carousel sections in `src/App.vue`
- **Styling**: Tailwind config in `tailwind.config.js`, global CSS in `src/assets/main.css`

> Folder name is **NetfliX**. If you want the npm package name to match, update `"name"` in `package.json`.

