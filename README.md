# Master Plan GeoRef Tool

A browser-based tool for georeferencing Indian city master plans. Collaborators match points between a master plan image and a satellite map to generate QGIS-compatible ground control point (GCP) files.

## How it works

1. Select a city from the dropdown to get the official master plan download link.
2. Upload the PDF/image to the tool (stays in your browser — never sent to any server).
3. Click matching points on the master plan and satellite map (5–7 points recommended).
4. Download the `.gcp` file and submit via GitHub Issue.

## For collaborators

No QGIS, no software install, no technical knowledge needed — just a browser.

1. Visit [the tool](https://sathvik6323.github.io/masterplan-overlay/)
2. Pick your city
3. Download the official PDF
4. Upload it and place 5–7 matching points
5. Download the GCP file
6. [Open an Issue](https://github.com/Sathvik6323/masterplan-overlay/issues/new/choose) and attach it

You'll be credited on the published map.

## For the maintainer

1. Download `.gcp` file from the Issue
2. QGIS → Raster → Georeferencer → Load GCP Points
3. Run transform → Export GeoTIFF
4. Deploy as Leaflet overlay

## Attributions

- Satellite tiles: [Esri World Imagery](https://www.esri.com/)
- PDF rendering: [PDF.js](https://mozilla.github.io/pdf.js/)
- Maps: [Leaflet](https://leafletjs.com/)

## License

Educational purpose. Master plans are property of their respective government bodies.
