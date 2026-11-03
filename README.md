# PUSH-IT · UTES site favourability map

![Funded by the European Union](assets/eu_funded_by.png)

An interactive map of underground thermal energy storage (UTES) favourability across Europe, built by the [University of Geneva](https://www.unige.ch/ge-rgba/) for [PUSH-IT](https://www.push-it-thermalstorage.eu/), a Horizon Europe project (Grant Agreement 101096566) on seasonal underground thermal energy storage.

This is Task 4.5's contractual deliverable, **D4.3, "GIS web-app for potential mapping"** (Horizon Europe PUSH-IT, M46). It is published here at an interim URL; the same application will also be embedded on the main PUSH-IT project website in coordination with EVIS.

## What this shows

Four favourability composites, one per underground thermal storage technology (ATES, HT-ATES, BTES, MTES), each combining multiple geological, hydrogeological, and demand-related indicators into a single 0–100 score per 10km grid cell across the EU27, UK, Switzerland, and Norway. Two data-coverage diagnostic layers show where the underlying indicators have valid data. PUSH-IT's six pilot sites (Delft, Darmstadt, Bochum, Berlin, Litoměřice, United Downs) are marked directly on the map.

## Data sources

The favourability composites are built from, and the map's basemap/context layers use:

- sEEnergies D5.1 District Heating Areas and D5.1 Industry Dataset (district heating areas, industrial excess heat), sEEnergies Open Data Hub, CC BY 4.0
- EEA Industrial Reporting, version 15 (large combustion plants and waste incinerators), European Environment Agency, CC BY 4.0
- Eurostat EU-SILC ilc_lvhe02 (national share of households on district heating, Norway and Switzerland)
- EEA WISE WFD (Water Framework Directive protected areas), European Environment Agency
- EEA Natura 2000 data, end 2020 (protected areas excluded from the maps), European Environment Agency
- EEA CORINE Land Cover 2018 (water bodies and wetlands excluded), Copernicus Land Monitoring Service
- IHME1500 (International Hydrogeological Map of Europe), BGR and UNESCO
- IGME5000 (International Geological Map of Europe and Adjacent Areas), BGR
- GISCO / Eurostat (population grid, country boundaries)
- Peta5.0.1 / sEEnergies, Heat Roadmap Europe (heat demand density), CC BY 4.0
- GeoERA RESOURCE (pan-European groundwater resources map)
- Global Heat Flow Database Release 2024, GFZ Potsdam, CC BY 4.0, DOI 10.5880/fidgeo.2024.014
- WorldClim 2.1 (surface temperature normals)
- OpenStreetMap contributors (mine/mineshaft locations, place labels)
- Natural Earth (country boundaries), public domain
- Basemap tiles: Esri, HERE, Garmin, FAO, NOAA, USGS

Full source-by-source access dates, methods, and exact usage are documented in the project's internal source log and are summarized in the PUSH-IT SMCA scientific report.

## Maintaining this site

This repository is published by GitHub Pages at **https://push-it.geoenergy.ch** from the `main` branch. Any change pushed to `main` goes live in 1–2 minutes; there is no build step.

- **Quick fix:** open the file on github.com (usually `index.html`), click the pencil icon, edit, and commit to `main`.
- **Larger change:** `git clone` the repo, preview with `python3 -m http.server 8000`, then commit and `git push`.
- **Do not delete the `CNAME` file**: it tells GitHub Pages which address serves this site.

Members of the geoenergy organization: the full guide (architecture, DNS, troubleshooting, who has access) is on the [organization page](https://github.com/geoenergy).

## Rights

© 2026 University of Geneva, PUSH-IT project. All rights reserved.

This repository publishes the deployed map application only. The data-processing pipeline and methodology used to build the favourability composites shown here (indicator selection, weighting, normalisation, and compositing) are not included in this repository and are not licensed for reuse. That methodology is documented in full in the PUSH-IT SMCA scientific report, available through the project.

No part of this repository (code or data files) may be copied, redistributed, or reused without prior written permission from the University of Geneva.

## Contact

Y. Makhloufi, [Geo-Energy, Reservoir Geology and Basin Analysis group](https://www.unige.ch/ge-rgba/), University of Geneva, Department of Earth Sciences.

---

Funded by the European Union. Views and opinions expressed are however those of the author(s) only and do not necessarily reflect those of the European Union or CINEA. Neither the European Union nor CINEA can be held responsible for them.
