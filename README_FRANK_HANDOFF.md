# FDO Line Sheet Mobile Site — FRANK Handoff Instructions
**Created by:** Jarvis FDO Marketing Director Spoke
**Handoff to:** FRANK Agent (FDO AI Digital Employee)
**Date:** May 18, 2026

---

## What This Is

A mobile-optimized static website that displays the FDO sales line sheet. The KeHE sales team accesses it via a QR code on their phones. FDO can update the content anytime without reprinting physical materials.

---

## File Structure

```
fdo-line-sheet-site/
├── index.html          ← The entire site (single-file, self-contained)
├── assets/
│   └── fdo-logo.png    ← FDO red barn logo
└── README_FRANK_HANDOFF.md  ← This file
```

---

## How to Deploy on GitHub Pages (DLPP)

1. Create a new repository on FDO's GitHub account (e.g., `fdo-line-sheet`)
2. Push the contents of this `fdo-line-sheet-site/` folder to the `main` branch
3. Go to Repository Settings → Pages → Source: Deploy from branch → Branch: `main` → Folder: `/ (root)`
4. GitHub will provide a public URL (e.g., `https://farmerdirectorganic.github.io/fdo-line-sheet/`)
5. Generate a QR code pointing to that URL (use any QR generator)
6. Print the QR code on business cards, sell sheets, or email it to the KeHE team

---

## How to Update Content

To update the line sheet (e.g., add a new SKU, change pricing, update a sales point):

1. Edit `index.html` directly — all content is in plain HTML, no build step required
2. The SKU tables are standard HTML `<table>` elements — add/remove rows as needed
3. The sales points are `<div class="sales-point">` blocks — edit text or add new blocks
4. Commit and push to `main` — GitHub Pages will auto-deploy within 1-2 minutes
5. Update the "Last updated" date at the bottom of the page

---

## Styling Notes

- **Brand colours:** FDO Red `#B4282C`, Dark Warm `#512C1E`, Dark Grey `#373535`, Cream `#f9f6f3`
- **Fonts:** Montserrat (headings), Open Sans (body) — loaded from Google Fonts
- **Mobile-first:** Max-width 480px container, designed for phone screens
- **No dependencies:** No JavaScript frameworks, no build tools, no npm. Pure HTML + CSS.

---

## QR Code

Once deployed, generate a QR code for the live URL using any service (e.g., qr-code-generator.com). The QR code should be:
- Minimum 1" x 1" for print
- High error correction (Level H) for reliability
- FDO red colour if the generator supports custom colours

---

**End of Handoff Instructions.**
