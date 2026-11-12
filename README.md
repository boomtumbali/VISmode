# IMGmode

**iPhone photos, any format. Private, quick and free.**
Live at **imgmode.vercel.app** · by [@boomtumbali](https://www.linkedin.com/in/boomtumbali/) · sister app of [PDFmode](https://pdfmode.vercel.app)

IMGmode turns iPhone HEIC photos into JPG, PNG, WebP or a PDF, and gives you the photo tools people use every day. Everything runs in your browser: your photos are never uploaded.

## Tools

| Tool | What it does |
| --- | --- |
| Convert photos | HEIC to JPG, or any photo to JPG, PNG, WebP or one PDF. Keep the date taken and camera if you like; location is always removed |
| Compress photos | Light, Balanced or Strong, with an optional "each photo under 2 MB / 1 MB / 500 KB" limit |
| Resize photos | Longest side 1080, 1600, 2048 or 4K, or 25/50/75%. Never enlarges |
| Crop & rotate | Original, 1:1, 4:5, 16:9, 3:2, 9:16 Story; drag to choose what stays; rotate and flip |
| Adjust & looks | Exposure, contrast, saturation, warmth, fade, vignette, and eight curated looks |
| Watermark | Your text in a corner, centred or repeated, in white, black or gold |
| Remove location | Shows which photos reveal where they were taken; removes location only (keeps date and camera) or everything. JPG and PNG keep every pixel |

After each export, IMGmode suggests a sensible next step and passes the photos you just made straight into it.

## Files

- **In:** HEIC/HEIF (iPhone, including Live Photo stills), JPG, PNG, WebP, GIF, BMP, AVIF, SVG. TIFF opens only in Safari.
- **Out:** JPG, PNG, WebP (where the browser can save it), PDF. Many photos come as one ZIP, each named like its original (`IMG_4021.jpg`).
- **Export names:** the first photo's name plus what was done, e.g. `IMG_4021-converted-by-imgmode.vercel.app.zip`.

## Privacy

No uploads, no sign-up, no ads. Photo details (location, camera, date) are shown before you share and removed by default.

## Good to know

- HEIC opens with the browser's own decoder in Safari, and with an open-source decoder (libheif, via `heic-to`) elsewhere. That decoder (about 3 MB) downloads the first time you open a HEIC photo, then stays cached.
- Very large batches work one photo at a time, so they take longer but don't run out of memory.
- Video (Live Photo motion, MOV, MP4) is planned for a later version.

## Host it

1. Create a GitHub repository (e.g. `IMGmode`) and upload `index.html` and this `README.md` (Add file → Upload files → Commit changes).
2. In Vercel: **Add New → Project**, import the repository, name the project `imgmode`, Framework Preset **Other**, no build command, then **Deploy**.

## Built with

[heic-to](https://github.com/hoppergee/heic-to) (LGPL-3.0, libheif) · [exifr](https://github.com/MikeKovarik/exifr) · [piexifjs](https://github.com/hMatoba/piexifjs) · [JSZip](https://stuk.github.io/jszip/) · [pdf-lib](https://pdf-lib.js.org) · Cormorant Garamond and Instrument Sans from Google Fonts. Libraries load from jsDelivr only when a tool needs them.
