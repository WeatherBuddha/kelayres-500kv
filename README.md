# Kelayres 500 kV Route Overlay

Interactive map: https://weatherbuddha.github.io/kelayres-500kv/

PPL Electric Utilities' open-house map for the proposed Kelayres 500 kV transmission line project
(Luzerne, Schuylkill, Carbon and Columbia counties, PA), georeferenced and overlaid on Google satellite
imagery so you can zoom in on the proposed Route A, B, C and D corridors.

- `index.html` — self-contained page (Leaflet, Google/Esri tiles, flyer image embedded). Opens offline from disk too.
- `kelayres_500kv_overlay.kmz` — the same overlay for Google Earth.

Alignment was fitted to the I-80 and I-81 centerlines with a 1° correction for scan tilt; expect up to about
0.1 mile of positional error near the map edges. The route bands on the flyer are schematic corridors, not
surveyed centerlines. Map source: PPL Electric Utilities open-house notice, October 2026.

## How it was made

PPL's flyer is just a picture of a map with no coordinates. Landmarks visible on it, mainly I-80 and I-81, were
matched against the known GPS positions of those highways from OpenStreetMap to work out how to stretch, shift and
slightly rotate the picture so everything lines up. The flyer is then shown as a see-through layer over Google's
satellite imagery.
