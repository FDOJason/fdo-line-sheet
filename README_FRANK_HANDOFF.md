# FDO KeHE 25 lb Line Sheet — Repository Handoff

**Site:** https://fdojason.github.io/fdo-line-sheet/
**Repository:** `FDOJason/fdo-line-sheet`
**Current published revision:** September 18, 2026
**Current PDF SHA-256:** `8fd0e77a35ca380594e0f21f8fa563e639ffcc7a0bee356215c125c72761afc7`

## Purpose

This repository publishes the mobile-optimized FDO KeHE 25 lb sales sheet reached by the permanent QR code printed on approved sales materials. The same stable QR destination can be reused by KeHE personnel and other authorized recipients; routine content updates do not require a new QR code.

## Current files

```text
fdo-line-sheet/
├── index.html
├── assets/
│   ├── KeHE_25lb.pdf
│   ├── fdo-linesheet-qr-permanent.png
│   └── fdo-logo.png
├── .github/workflows/static.yml
└── README_FRANK_HANDOFF.md
```

The September 17 three-page PDF was replaced on September 18, 2026 by the corrected four-page version containing the Our Story. Our Farmers. page and the Jason Thon attribution. The live asset uses the short Windows-safe filename `KeHE_25lb.pdf`. Git history preserves prior revisions if restoration is ever required.

## Publishing workflow

1. Make approved content changes in `index.html`.
2. Add the approved PDF under `assets/` with a dated, descriptive filename.
3. Confirm the PDF download link in `index.html` points to the current approved file.
4. Verify the permanent QR decodes to `https://fdojason.github.io/fdo-line-sheet/`.
5. Remove the superseded PDF from the live branch after approval.
6. Commit and push to `main`; GitHub Pages deploys through `.github/workflows/static.yml`.
7. Verify the GitHub Pages workflow succeeds, the live HTML shows the approved copy, the current PDF returns HTTP 200, and the removed PDF returns HTTP 404.

## Visual system

- **FDO red:** `#B4282C`
- **Dark warm:** `#512C1E`
- **Dark grey:** `#373535`
- **Cream:** `#f9f6f3`
- **Headings:** Montserrat
- **Body:** Open Sans
- **Layout:** mobile-first, maximum width 480 pixels

## QR longevity

`assets/fdo-linesheet-qr-permanent.png` encodes the permanent GitHub Pages URL, not a temporary Manus or sandbox address. It is suitable for repeated distribution as long as the GitHub Pages site and repository remain active. Update the webpage and PDF in place rather than changing the QR destination.
