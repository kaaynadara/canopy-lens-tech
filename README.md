# Canopy Lens

Canopy Lens is a lightweight, browser-based dashboard for exploring aerial forest imagery. Upload an image to estimate green canopy coverage, approximate canopy area, annual CO₂ potential, and an estimated crown count.

## Run locally

No setup or installation is required.

1. Open `index.html` in a modern browser.
2. Upload an aerial or top-down forest image, or select **Try with a generated sample**.
3. Adjust the ground resolution and canopy-colour controls as required.
4. Download the results as a CSV report.

## Features

- Image upload for JPG and PNG files
- Interactive green-canopy mask
- Adjustable hue, saturation, brightness, and ground-resolution controls
- Estimated canopy cover, area, tree crowns, and annual CO₂ potential
- Land-cover donut chart
- English, Hindi, and Bengali interface options
- CSV export
- Responsive browser interface

## Tech stack

- HTML5
- CSS3
- Vanilla JavaScript
- Canvas API for browser-side pixel analysis and mask rendering
- Google Fonts: DM Sans, DM Mono, Playfair Display, Noto Sans Bengali, and Noto Sans Devanagari

## Important limitations

This is a client-side prototype. The canopy result is based on HSV-style colour segmentation in the browser; it is most useful for clear aerial/top-down imagery with visible vegetation. It does **not** use a trained tree-crown detection model, GIS coordinates, or verified carbon methodology.

Tree count and carbon figures are estimates, not validated measurements. Ground-level images, shadows, water, soil, seasonal colour changes, and an incorrect meters-per-pixel setting can produce misleading results. Use it for exploration and demo purposes, not carbon-market reporting or scientific decisions.

## Project structure

```text
canopy-lens/
├── index.html   # Complete responsive web application
└── README.md    # Project documentation
```
