# Safrael Site

A clean, responsive personal site built with pure HTML and CSS. It includes a profile sidebar with skills, quick links, a projects section, and helpful widgets—all wrapped in a modern animated gradient theme.

---

## Overview

The layout uses CSS Grid to form three columns on desktop (Aside | Main | Ads), collapses to two columns on tablets around 768px, and stacks into a single column on phones. The header is sticky with a glass-effect background; cards and widgets use subtle shadows and hover effects for a polished look.

## Features

- Pure HTML + CSS (no frameworks)
- Responsive layout targeting mobile, tablet (768px), and desktop
- Sticky header with blur and animated gradient background
- Profile sidebar with image, name, role, and skills
- Projects section using simple, reusable cards
- Widgets: Newsletter subscription and Trending topics
- Keyboard-focusable links and buttons

## Tech Stack

- HTML5
- CSS3 (Grid, Flexbox, keyframes)

## Project Structure

```
Site-practise/
├─ index.html      # Markup structure
├─ style.css       # Styling and responsive rules
└─ .vscode/
   └─ settings.json  # Optional editor settings
```

## Responsive Behavior

- Mobile (≤ 767px): single-column flow: Header → Main → Aside → Ads → Footer
- Tablet (768–1023px): two columns (Aside | Main). Ads and Footer span full width.
- Desktop (≥ 1024px): three columns (Aside | Main | Ads) with footer full width.

Guidelines followed:
- Avoid fixed heights on grid rows; let content size naturally
- Scale media: `img { max-width: 100%; height: auto; }`
- Allow navigation to wrap on smaller screens

## Getting Started

Open `index.html` directly in your browser, or run a small local server for cleaner testing.

### Preview locally (Windows PowerShell)

```powershell
# Python 3
python -m http.server 8000

# Node.js
npx http-server -p 8000
```
Then open http://localhost:8000 and navigate to this project folder.

## Customization

- Colors: Edit the gradient in `body` and component backgrounds in `style.css`
- Spacing: Adjust gaps and paddings in `.container`, `header`, `main`, `aside`, `.projects`
- Cards: Tweak `.project-card` and button styles
- Breakpoints: Update `@media` queries if you target different devices

## Deployment

Host the static files on any platform:
- GitHub Pages
- Netlify
- Vercel
- Cloudflare Pages

GitHub Pages quick start:
1. Push the folder to a GitHub repository
2. In Settings → Pages, set Source to the `main` branch root
3. The site will be available at `https://<username>.github.io/<repo>/`

## Screenshots (optional)

Place screenshots under `assets/` to showcase desktop, tablet, and mobile views.

```
assets/
├─ desktop.png
├─ tablet-768.png
└─ mobile.png
```

Reference them here:
- Desktop: `assets/desktop.png`
- Tablet (768px): `assets/tablet-768.png`
- Mobile: `assets/mobile.png`

## Roadmap

- Link project cards to live demos
- Improve accessibility (skip links, visible focus states)
- Optional dark mode
- Minify CSS for production

## License

This project is licensed under the MIT License — see the `LICENSE` file for details.
