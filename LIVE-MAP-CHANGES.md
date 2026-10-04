# SENTINEL Live Map changes

- Map is draggable and zoomable with MapLibre + OpenStreetMap.
- Impact areas are geographic GeoJSON polygons with Critical / Severe / Warning bands. They stay anchored to the incident coordinates when the map is dragged or zoomed.
- Real Mumbai facilities are shown as map markers: Shatabdi Hospital, Kokilaben Hospital, Nanavati Max, Cooper Hospital, Holy Spirit Hospital, Kandivali Police Station, Bandra Fire Station, K/East Mini Fire Station, hospital blood banks, and Indian Red Cross Society.
- Facility names/locations are real. Bed/ICU/blood/ambulance values remain simulation data for the hackathon and should not be interpreted as live public-safety data.
- Road corridors are geographic line features with state colors: green=open, yellow=slow, orange=damaged, red=blocked, purple=high-risk.
- Dashboard has 1x / 2x / 5x / 10x controls. Speed is stored in browser localStorage and survives page refreshes.
- Run Simulation, Adapt Model, Start Demo, Recalculate Now, and Adapt Model To Situation are wired to visible state updates and alerts.
- Google Maps is linked from the map for the same incident location. A fully embedded Google Maps basemap would require a Google Maps JavaScript API key; this build intentionally avoids requiring or exposing an API key.
