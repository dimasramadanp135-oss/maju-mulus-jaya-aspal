# Maju Mulus Jaya Aspal — Static Site

## Overview
Single-page Indonesian-language marketing site for an asphalt paving / road painting service company (Maju Mulus Jaya Aspal). The site is a single static `index.html` plus image assets at the project root.

## Project Structure
- `index.html` — full single-page site (HTML + inlined CSS + inlined JS)
- `logo.png`, `aspalbackground.jpg`, `portfolio_1..4.jpg` — static image assets referenced from `index.html`

## Tech Stack
- Plain static HTML/CSS/JS (no build step, no framework, no package manager)

## Replit Setup
- Workflow `Start application` serves the project root via Python's built-in HTTP server:
  - Command: `python3 -m http.server 5000 --bind 0.0.0.0`
  - Port: `5000` (the only externally exposed port)
- Deployment is configured as a `static` deployment with `publicDir = "."`.

## Notes
- A 404 for `/favicon.ico` is harmless — no favicon file is provided and none is referenced from the HTML.
