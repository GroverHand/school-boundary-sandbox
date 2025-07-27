# School Boundary Sandbox

Client-side web app to:
- Upload a CSV of students (either LAT/LON or ADDRESS/CITY/STATE/ZIP)
- Plot pins on a Leaflet map
- Draw polygon/rectangle to select students
- Show a summary panel (counts by fields, numeric stats)
- Export selected rows to CSV

## Run locally
Just open `index.html` in Chrome/Edge/Firefox. No server required.

## Column rules
- Preferred: `LAT` and `LON` (or `LNG`) columns (fast, no geocoding).
- Or: `ADDRESS`, `CITY`, `STATE`, `ZIP` (the app will geocode via Nominatim at ~1 req/sec).

## Vendor libraries
Currently loaded from CDNs. If your network blocks them, place local copies in `/vendor` and update the script tags:
- leaflet.js / leaflet.css
- leaflet.draw.js / leaflet.draw.css
- papaparse.min.js
- turf.min.js

## Privacy note
No data is transmitted to a server by this app. Everything happens in your browser.

## License
MIT
