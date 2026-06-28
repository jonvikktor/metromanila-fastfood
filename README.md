# Cornering the Competition: How Jollibee and McDonald's Keep Opening Side by Side in Metro Manila

## Goal
With the Philippines' two biggest fastfood chains -- Jollibee and McDonald's -- frequently located close to each other, I mapped and analyzed the proximity of their branches across Metro Manila to find out how often the two end up as neighbors.

The data shows that Jollibee and McDonald's frequently co-locate across Metro Manila. Nearly 70% of Jollibee branches have a McDonald's within 500 meters. The closest pair, at Venice Grand Canal Mall in Taguig, are just 10.7 meters apart.

## Methodology
Branch location data was collected via the Google Maps Places API in June 2026. Searches were run for each of the 17 cities and municipalities of the National Capital Region separately as a workaround, given the API's 60-result-per-search limit.

Branches were then deduplicated using coordinate rounding (four decimals). City names were extracted from formatted addresses. Distances between Jollibee and McDonald's branches were calculated using the Haversine formula.

Maps were done on QGIS, with labels made on Adobe Illustrator.

## Disclaimer
This was my first time using the Google Maps Places API and building a scrollytelling page from scratch. The Haversine formula was done in Python, as recommended by Google. The Google Maps Places API occasionally returned branches with coordinates slightly outside the NCR administrative boundary, even with a restriction bounding box.

## For future me (With more time)
- Increase dot size on the maps for better readability
- Add an inset locator map showing NCR within the Philippines

## Live page
[https://jonvikktor.github.io/metromanila-fastfood](https://jonvikktor.github.io/metromanila-fastfood)
