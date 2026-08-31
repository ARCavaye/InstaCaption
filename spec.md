# InstaCaption
A simple tool to generate correctly formatted captions for my Instagram posts.

Uses values submitted via a form to complete a template caption. Applies instagram-compatible whitespace to ensure it displays correctly/

## Caption format
```
[CAPTION]

📸 [CAMERA (default: Canon R6ii)] + [LENS (default:RF 100-500mm f4.5-7.1L)]
🏷️ [ANIMAL]
📍 [LOCATION]

[HASHTAGS (as many as required)]
```

## Blank Lines
Blank lines have a Unicode “Braille Pattern Blank” character (U+2800) inserted so that Instagram does not truncate them.

## Dependencies
Prefer dependenceis that can be loaded from a CDN.