# Master Plan GeoRef Tool

**[Launch the Tool →](https://sathvik6323.github.io/masterplan-overlay/)**

A browser-based tool for georeferencing Indian city master plans. Collaborators match points between a master plan image and a satellite map to generate QGIS-compatible ground control point (GCP) files. Supports **120+ ULBs** across Andhra Pradesh.

## Features

- **Search & zoom** — type your city name to search, select it, and the map flies to its location
- **120+ cities** — official master plans for all Andhra Pradesh Urban Local Bodies
- **PDF & JPG support** — render PDFs via PDF.js or load PNG/JPG images
- **Image zoom/pan** — scroll-wheel zoom, drag-to-pan, pinch-zoom on touch devices
- **GCP upload verification** — load a `.gcp` file to visually verify points on both panels
- **Session save/restore** — your work is saved in the browser; pick up where you left off
- **Basemap switcher** — toggle between satellite and street map views

## How it works

1. **Search your city** — type in the search box, select your city, and download the official master plan.
2. **Upload the file** — drag it onto the left panel or click "Choose File" (PDF, PNG, JPG).
3. **Place GCP points** — click a landmark on the master plan, then click the same spot on the map. Repeat at least **10 times** with points spread across the area.
4. **Download GCP** — export the `.gcp` file for QGIS. Or **Upload GCP** to verify someone else's points.

## For collaborators

No QGIS, no software install, no technical knowledge needed — just a browser.

1. Visit [the tool](https://sathvik6323.github.io/masterplan-overlay/)
2. Search and pick your city
3. Download the official PDF/JPG
4. Upload it and place **10+** matching points
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
- Geocoding: [Nominatim](https://nominatim.openstreetmap.org/) (OpenStreetMap)
- **Master Plan Source**: [Directorate of Town & Country Planning, Govt. of Andhra Pradesh](https://dtcp.ap.gov.in/)

## License

Educational purpose. Master plans are property of their respective government bodies.
