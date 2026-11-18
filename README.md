# Iowa officials embed widget · V5

Use embed.html inside a custom HTML/code block that allows scripts, styles, and external libraries. Add once per page. Alternatively upload index.html to static hosting and embed that URL using an iframe. No backend, build step, API key, or database connection is needed. Internet access is needed for Leaflet and OpenStreetMap background tiles.

V4 removes the page header and footer and merges the V2 county assignments into five region outlines. At the statewide view, clicking a region zooms into that area and filters the officials to that roster. Inside a region, overlays are hidden and no longer intercept clicks. Pan and zoom to inspect towns and click dots for contact details. The All Iowa button returns to regional selection. Region dropdown labels use short names with a spaced custom chevron, including on phones.

The roster remains at 160 entries, including 114 explicitly certified starters. Data handling and contact exceptions are unchanged from V2. Street addresses are omitted. Pins remain approximate ZIP-area points, with one city-level fallback. Keep the master roster separately; changes there do not automatically update this snapshot.

The regional footprints retain the previously inferred V2 assignments, merged into continuous shapes; no official boundary verification has been added. Tooltips use the region name only, as requested.

Sources: five supplied regional officials PDFs; 2025 U.S. Census ZCTA Gazetteer; Census TIGERweb Iowa state and county outlines. Leaflet 1.9.4 from unpkg; © OpenStreetMap contributors. Keep attribution visible and follow https://operations.osmfoundation.org/policies/tiles/ .

V4 adds a colored Reset filters button in the top-right map toolbar. Both reset buttons clear search and region selection and restore the certified-starters filter. Selected regions retain their fill color and outline, with pointer events disabled so they do not intercept clicks. Selecting a region starts one zoom level closer than the V3 region-bounds view; edges may fall outside the initial viewport. Pan, zoom out, or choose Show results to see the full spread of officials.

## V5 updates
On viewports up to 760 px wide, clicking a dot or a result opens contact details in a centered modal dialog above the map controls. The dialog scrolls internally, closes with the close button, Escape, or a backdrop click, and supports shared-ZIP lists. Desktop retains anchored map popups. The display label for records whose certified flag is false is now Standard Official. This is a display classification; source certification fields have not been changed or newly verified.

## Opening the download on a Mac
Unzip and double-click Start local preview.command. Keep its Terminal window open while viewing the map. It uses Python 3 and binds only to localhost. Raw file previews omit the background tiles because they cannot provide the web referrer required by the tile service. On your website, serve the embed over HTTPS and allow referrer headers for the tile requests.
