# Eric Tang — Portfolio

**Live site:** https://erictang0220.github.io/My-Portfolio/

Personal portfolio showcasing my software engineering experience, projects, and Chinese calligraphy/brush painting artwork.

## Features

- **Work history** — DoorDash, Amazon, Cruise, and other experience
- **Projects** — software engineering projects with links to repos where public
- **Art gallery** — carousel + full grid of Chinese calligraphy and brush painting pieces
- **Contact form** — powered by Web3Forms (no backend required)
- Smooth scroll navigation, responsive layout

## Tech Stack

- React (class components), Create React App
- `react-multi-carousel` for art carousel
- `react-reveal` for scroll animations
- Web3Forms for contact form submission
- Deployed on GitHub Pages (`gh-pages` branch)

## Data

All content is data-driven — edit `public/resumeData.json` to update bio, work history, skills, projects, and artwork without touching React code.

## Local Development

```bash
git clone https://github.com/erictang0220/My-Portfolio
cd My-Portfolio
npm install
npm start
```

## Deploy

```bash
NODE_OPTIONS=--openssl-legacy-provider npm run build
NODE_OPTIONS=--openssl-legacy-provider ./node_modules/.bin/gh-pages -d build
```

> Note: `npm run deploy` does not work directly — `predeploy` doesn't inherit `NODE_OPTIONS` on Node v25+.
