# Journal Poster Generator

A static, single-page web app that renders an A3 portrait academic poster with an Apple Liquid Glass aesthetic and exports the design to high-resolution PNG or PDF.

## Getting started
1. Serve the folder (or open `index.html` directly). Using Python:
   ```bash
   python -m http.server 8000
   ```
2. Open `http://localhost:8000` in your browser.

## Usage
- The poster is previewed at a reduced scale for screens; the export runs at full A3 size (3508×4961 px, 300 DPI target).
- Use **Download PNG (A3)** or **Download PDF (A3)** to export print-ready files. The capture routine removes preview scaling, renders with `html2canvas` (scale 2), and writes the A3-sized canvas to jsPDF.
- Design tokens (colors, shadows, blur) are defined in the `<style>` block and implement the frosted glass look with `backdrop-filter`, translucent surfaces, and soft gradients.

## Notes
- All assets are pulled via CDN (`html2canvas`, `jsPDF`, and Inter font), so no build tooling is required.
- Print styles hide the control bar and disable scaling for direct printing.
