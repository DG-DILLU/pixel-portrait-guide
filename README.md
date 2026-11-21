# Portrait / Grid

A local-first portrait drawing guide. It turns a photo into an interactive, color-reduced grid fitted to A4, with coordinates, color and pencil suggestions, a completion checklist and PDF downloads.

## Run

Open `index.html` in a current desktop or mobile browser. No installation, server, dependencies or account are required. The Google Fonts link is optional; the application remains usable offline with fallback fonts. Uploaded images are processed in the browser and are never sent to a server.

## Workflow

1. Choose or drop a JPG, PNG or WEBP image (up to 25 MB).
2. Select portrait or landscape A4, drawing detail and palette size.
3. Use crop zoom and position sliders to frame the subject.
4. Click a square to inspect its coordinate, average color, HEX and pencil suggestion. Mark squares complete in the inspector or coordinate checklist.
5. Download an A4 grid, pixel reference, coordinate grid or palette and instruction sheet. Print measured grids at **100% / Actual size** and disable “Fit to page.”

## A4 measurement

The image is fitted without stretching inside 15 mm minimum margins. The drawing area's dimensions are constrained by A4 printable bounds and the image aspect ratio. Column count sets the row count by rounding columns divided by source aspect ratio. Printed cells may be rectangular to preserve the image proportions; the interface reports each exact side in millimetres. At the offered detail settings, the grid is sized to fit on one A4 page.

## Image processing

Canvas resampling averages each grid cell. The 8, 12, 16 and 24 color options use weighted median-cut quantization; “Original colors” retains per-cell averages. PDF documents are generated locally.
