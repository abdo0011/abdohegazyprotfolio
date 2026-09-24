# Abdo Elrhman Hegazy — Cybersecurity Portfolio (React + Vite)

A React + Vite conversion of the original single-page portfolio. Same design,
same content, same animations — now split into clean, reusable components.

## Getting started

```bash
npm install
npm run dev
```

Open the printed local URL (typically http://localhost:5173) in your browser.

## Adding your real profile photo

1. Save your photo as `profile.jpg`.
2. Place it in `public/images/profile.jpg`.
3. Reload the page — the Hero section will show it automatically.

No code changes are required. If the file is missing, the site falls back to
the existing neutral placeholder icon (never a generated or invented photo).

## Project structure

```
├── index.html               # HTML entry point, fonts
├── public/
│   └── images/               # Put profile.jpg here
├── src/
│   ├── main.jsx               # React entry point
│   ├── App.jsx                 # Composes all sections
│   ├── index.css                # Global styles (design system, unchanged)
│   ├── data/
│   │   └── content.js            # All factual copy in one place
│   ├── hooks/
│   │   └── useReveal.js           # Scroll-reveal animation hook
│   └── components/
│       ├── Navbar.jsx              # Sticky nav + mobile menu
│       ├── Reveal.jsx               # Scroll-reveal wrapper
│       ├── ProfilePhoto.jsx          # Photo with placeholder fallback
│       ├── Hero.jsx
│       ├── About.jsx
│       ├── Education.jsx             # Education + Current Training
│       ├── Skills.jsx
│       ├── Tools.jsx
│       ├── Projects.jsx
│       ├── Certifications.jsx
│       ├── Journey.jsx                # Learning journey timeline
│       ├── Writeups.jsx
│       ├── Contact.jsx
│       └── Footer.jsx
```

## Updating content

All text — skills, tools, projects, certifications, timeline steps, and
write-up titles — lives in `src/data/content.js`. Edit that file rather than
the components to keep things consistent and to avoid touching markup.

## Build

```bash
npm run build
npm run preview
```

`npm run build` outputs a production build to `dist/`.
