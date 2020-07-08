# Country Bounding Boxes

A list of 240+ country, city-state and region bounding boxes. Kept in JSON with ISO 3166-1 code as key.
Useful when zooming a map to a specific country in Mapbox, Google Maps or similar services.

The boxes are confined to the primary area for each country. Outlying territory are excluded 
(for example, the US bounding box does not contain Pacific islands such as Guam).

Feel free to PR suggested changes (bounding boxes for missing countries or updates to existing boxes).

## Data structure

```json
{
    "ISO_country_code": [
      "country_name",
      [
        min_lon,
        min_lat,
        max_lon,
        max_lat,
      ],
    ]
  }
```

## Example

```json
{
  "PL": ["Poland", [14.07, 49.03, 24.03, 54.85]],
  "PM": ["Saint Pierre and Miquelon", [-56.41, 46.75, -56.12, 47.14]],
  "PN": ["Pitcairn", [-130.73, -25.07, -124.78, -23.92]],
  "PR": ["Puerto Rico", [-67.24, 17.95, -65.59, 18.52]],
  "PS": ["West Bank", [34.93, 31.35, 35.55, 32.53]],
  "PT": ["Portugal", [-9.53, 36.84, -6.39, 42.28]],
  "…"
}
```

## Sources

- http://www.naturalearthdata.com (110m cultural vectors, admin 0)
- https://nominatim.openstreetmap.org/
- https://wiki.openstreetmap.org/wiki/User:Ewmjc/Country_bounds
- my manual fixups

## License
Public Domain
