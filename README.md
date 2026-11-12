# VISmode

**iPhone photos, any format. Private, quick and free.**

**Use it now at [vismode.vercel.app](https://vismode.vercel.app)**: nothing to install, no sign-up. Works on phones, tablets and computers in Safari, Chrome, Edge and Firefox.

By [@boomtumbali](https://www.linkedin.com/in/boomtumbali/) · sister app of [PDFmode](https://pdfmode.vercel.app) for PDFs

VISmode turns iPhone HEIC photos into JPG, PNG or WebP and gives you the photo tools people use every day. Everything runs in your browser: your photos are never uploaded.

## Tools

| Tool | What it does |
| --- | --- |
| Convert photos | HEIC to JPG, or any photo to JPG, PNG or WebP. Can keep the date taken and camera; location is always removed |
| Photos to PDF | One PDF, one photo per page, in your order. Pages fit each photo, or A4 / Letter |
| Compress photos | Light, Balanced or Strong, with an optional "each photo under 2 MB / 1 MB / 500 KB" limit |
| Resize photos | Longest side 1080, 1600, 2048 or 4K, or 25/50/75%. Never enlarges |
| Crop & rotate | Original, 1:1, 4:5, 16:9, 3:2, 9:16 Story; drag to choose what stays; rotate and flip |
| Add a border | Fit the whole photo in a square, 4:5, Story or 16:9 frame with a white, black or blurred border. No cropping |
| Adjust & looks | Exposure, contrast, saturation, warmth, fade, vignette, and eight looks |
| Watermark | Your text in a corner, centred or repeated, in white, black or violet |
| Remove location | Shows which photos reveal where they were taken; removes location only (keeps date and camera) or everything. JPG and PNG keep every pixel |

After each export, VISmode suggests a sensible next step and passes the photos you just made straight into it.

## Files

- **In:** HEIC/HEIF (iPhone, including Live Photo stills), JPG, PNG, WebP, GIF, BMP, AVIF, SVG. TIFF opens only in Safari.
- **Out:** JPG, PNG, WebP (where the browser can save it), or PDF. Many photos come as one ZIP, each named like its original (`IMG_4021.jpg`).
- **Export names:** the first photo's name plus what was done, e.g. `IMG_4021-converted-by-vismode.vercel.app.zip`.

## The start-page film

Until a video is added, the start page plays a short film made in code (no download, follows light and dark mode, pauses off screen, and stays still for people who turn off motion). To use a real video, upload `vismode-promo-1080p.mp4` (and optionally `vismode-promo-1080p.webm` and `vismode-poster.jpg`) next to `index.html`. The page detects it and plays it instead, with sound and full-screen buttons, like PDFmode.

## Good to know

- HEIC opens with the browser's own decoder in Safari, and with an open-source decoder (libheif, via `heic-to`, about 3 MB) elsewhere. It downloads the first time you open a HEIC photo, then stays cached.
- Large batches are processed one photo at a time: slower, but they don't run out of memory.
- Video (Live Photo motion, MOV, MP4) is planned for a later version.

## Files

- `index.html`: the whole app.
- `og-image.png`: the picture shown when the link is shared on Messenger, Facebook, X and other apps.

## Updating the live site

vismode.vercel.app is built from this repository. To publish an update, upload the new `index.html` (and this `README.md`) here with Add file → Upload files → Commit changes; Vercel deploys it automatically within a minute. After changing `og-image.png`, Messenger and Facebook may keep showing the old picture until you press **Scrape Again** at developers.facebook.com/tools/debug.

## Built with

[heic-to](https://github.com/hoppergee/heic-to) (LGPL-3.0, libheif) · [exifr](https://github.com/MikeKovarik/exifr) · [piexifjs](https://github.com/hMatoba/piexifjs) · [JSZip](https://stuk.github.io/jszip/) · [pdf-lib](https://pdf-lib.js.org) · Arvo and Inter from Google Fonts. Libraries load from jsDelivr only when a tool needs them.
