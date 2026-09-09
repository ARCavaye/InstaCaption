# InstaCaption

A simple, single-page tool for generating correctly formatted captions for Instagram posts. Fill in a form with your caption, camera, lens, subject, location, and hashtags, and get an Instagram-ready caption you can copy with one click.

## Features
- Live preview of the formatted caption as you type
- Instagram-safe blank lines (uses U+2800 Braille Pattern Blank so line breaks aren't collapsed)
- Sensible defaults for camera (Canon R6ii) and lens (RF 100-500mm f4.5-7.1L)
- Hashtag input accepts space/comma/newline-separated tags and normalizes the `#` prefix
- One-click copy to clipboard
- Installable as a Progressive Web App (PWA) that works offline

## Caption format
```
[CAPTION]

📸 [CAMERA (default: Canon R6ii)] + [LENS (default: RF 100-500mm f4.5-7.1L)]
🏷️ [SUBJECT]
📍 [LOCATION]

[HASHTAGS (as many as required)]
```

## Running locally
The app is a single static HTML file with no build step. Just open `index.html` in a browser, or serve it with any static file server.

## Running with Docker
```sh
docker build -t instacaption .
docker run -p 8080:80 instacaption
```
Then visit `http://localhost:8080`.

## Installing as an app
- **iOS Safari**: Share → Add to Home Screen
- **Android Chrome**: Menu → Install app (or Add to Home screen)

## Dependencies
All dependencies are loaded from a CDN (Google Fonts, Lucide icons) — no local install or build tooling required.
