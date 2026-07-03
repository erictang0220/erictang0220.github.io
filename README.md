# Eric Tang -- Portfolio

Personal portfolio site showcasing software engineering experience, projects, and Chinese calligraphy and brush painting artwork.

**Live site:** https://erictang0220.github.io/

## Overview

A single-page React application with smooth-scroll navigation, scroll-triggered animations, and a responsive art gallery carousel. All content is data-driven through a single JSON file, so bio, work history, skills, projects, and artwork can be updated without touching React source code.

## Sections

| Section | Description |
|---|---|
| Header | Name, tagline, and social links |
| About | Bio and skills summary |
| Resume | Education and work experience |
| Art Gallery | Carousel of Chinese calligraphy and brush painting pieces |
| Contact | Contact form |

## Tech Stack

- **Framework:** React 17 (class components), Create React App
- **Data source:** `public/resumeData.json` and `public/artwork.json`
- **Art carousel:** `react-multi-carousel` with responsive breakpoints (1/2/3 items by viewport width)
- **Animations:** `react-reveal` (Fade, Slide) for scroll-triggered transitions
- **Analytics:** `react-ga` (Google Analytics)
- **Deployment:** GitHub Pages via `gh-pages` branch

## Local Development

```bash
git clone https://github.com/erictang0220/erictang0220.github.io
cd erictang0220.github.io
npm install
npm start
```

## Deploy

```bash
NODE_OPTIONS=--openssl-legacy-provider npm run build
NODE_OPTIONS=--openssl-legacy-provider ./node_modules/.bin/gh-pages -d build
```

> Note: `NODE_OPTIONS` must be set explicitly on Node v17+ due to OpenSSL legacy provider requirements. The `npm run deploy` shortcut does not propagate this env var through the `predeploy` hook.

## Updating Content

Edit `public/resumeData.json` to update bio, work history, skills, and projects. Edit `public/artwork.json` to add or remove art pieces. No React code changes required.

