# Niagara Interactive Map — v0.83

GitHub Pages package for the Niagara industrial and radiological history map.

## v0.83 update

- The historical-map canvas is now black, so missing or transparent aerial tiles appear black instead of beige or white.

- Restored Rattlesnake Creek with a revised trace based on the supplied USACE map
- Restored Two Mile Creek from the Niagara River south to the Kenmore Avenue area
- Added clickable popups with radiological context and supporting DOE/NYSDEC links
- Added separate legend and layer-control entries for the two waterways
- Retained clear warnings that the traces are approximate documentary overlays, not surveyed GIS centerlines or contamination boundaries

Upload all files to the repository root and publish GitHub Pages from the `main` branch and `/ (root)`.


## v0.83 waterway correction
Two Mile Creek was shifted west to follow the mapped channel beside Two Mile Creek Road, under I-290, through Sheridan Park, and toward Kenmore Avenue. Rattlesnake Creek was redrawn as the western tributary through Tonawanda North Unit 2.


## v0.83 waterway update
- Rattlesnake Creek geometry retained.
- Two Mile Creek now winds through Sheridan Park and Sheridan Park Golf Course and bends southeast toward the former Linde area.
- Waterway lines remain approximate documentary overlays, not surveyed GIS centerlines.


## v0.83
- Radiation guide button changed to black with white lettering.
- Historical NHAP imagery is now the opening basemap.
- At zoom level 16 and closer, the map automatically switches to the modern street map; zooming back out returns to the historical aerial.


## v0.83 display correction
The NHAP tile service contains white pixels inside some raster tiles, rather than transparent gaps. This version applies a luminance-based transparency filter to white and near-white historical-map pixels, revealing the black map background underneath. At close zoom, the map still switches to the modern street basemap.

- v0.83 aligns the Radiation guide button horizontally with the map layer/legend control.


Version 0.60 starts at a fixed Niagara corridor view, enables the 1978–1979 aerial survey layer by default, and moves editable styling into style.css.


## v0.83 opening view correction
- Uses a sidebar-aware horizontal offset after the map layout is measured.
- Opens at zoom 12 with the Niagara corridor shifted right into the visible map area, matching the supplied screenshot more closely.
- The 1978–1979 aerial radiological survey remains enabled at startup.


Panel frame controls are located at the very bottom of style.css. Edit --panel-frame-size and --panel-frame-color there.
