# Iowa officials widget · V9

V9 replaces the map engine completely with MapLibre GL JS 5.6.2 and the OpenFreeMap Liberty vector basemap. No previous map engine or public raster tile endpoint is loaded.

Upload index.html to GitHub Pages or other HTTPS static hosting. Alternatively paste embed.html into one custom HTML block that permits inline JavaScript/CSS and the external resources. No backend, build process, or API key is required. Internet access and a WebGL-capable browser are required.

Your host must allow unpkg.com, tiles.openfreemap.org, the sources referenced by its style, and the MapLibre worker (blob:). Keep all background-map attribution visible. See https://openfreemap.org/quick_start/ and https://maplibre.org/ .

The 160 embedded records, five region outlines, standard-official classification, centered mobile contact dialog, custom closed-on-map-click region picker, and V7 filter-preserving view buttons remain. Region selection starts closer in; Show Region fits its outline. Show Iowa changes the camera only. Reset Filters restores All Iowa, clears search, and checks certified starters.

For local preview, unzip and double-click Start local preview.command on this Mac. Python 3 is needed; keep the Terminal window open. Local preview is not required on GitHub Pages. Source rosters do not automatically sync into the HTML.

Regions retain the previously inferred footprints. Positions are approximate ZIP representative points, with the existing Davenport city fallback. Street addresses are excluded from the widget. Bill Neal's duplicate was consolidated; the two possible Alecia duplicates remain. Justin Parson's phone remains unavailable in the public card until verified.
