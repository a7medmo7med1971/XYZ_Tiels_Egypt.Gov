# Egypt Governorates XYZ Tiles Layer

This repository provides an **XYZ Tiles** web map layer representing the Governorates of Egypt. The layer was generated from an original shapefile using **QGIS** and is optimized for Web GIS applications to ensure fast loading, smooth rendering, and efficient performance.

---

## Overview

### Coverage

All Governorates of the Arab Republic of Egypt.

### Coordinate Reference System (CRS)

`EPSG:3857 - Web Mercator`

### Zoom Levels

`5 – 11`

### Format

`PNG` with transparency support, allowing the layer to be overlaid on any basemap.

---

## Tile URL

You can integrate this layer directly into web mapping applications such as Leaflet, OpenLayers, or Mapbox using the following URL:

```text
https://a7medmo7med1971.github.io/XYZ_Tiels_Egypt.Gov/{z}/{x}/{y}.png
```

If the generated tiles are stored inside a subfolder (for example, `egypt_tiles`), use:

```text
https://a7medmo7med1971.github.io/XYZ_Tiels_Egypt.Gov/egypt_tiles/{z}/{x}/{y}.png
```

---

## Leaflet Example

```javascript
const egyptLayer = L.tileLayer(
    'https://a7medmo7med1971.github.io/XYZ_Tiels_Egypt.Gov/{z}/{x}/{y}.png',
    {
        minZoom: 5,
        maxZoom: 11,
        opacity: 0.8,
        attribution: '© Egypt Governorates XYZ Tiles'
    }
).addTo(map);
```

---

## Use Cases

* Web GIS Applications
* Interactive Dashboards
* Government and Administrative Mapping
* Spatial Analysis Platforms
* Educational and Research Projects

---

## Data Specifications

| Property     | Value              |
| ------------ | ------------------ |
| Coverage     | Egypt Governorates |
| CRS          | EPSG:3857          |
| Tile Format  | PNG                |
| Transparency | Supported          |
| Min Zoom     | 2                  |
| Max Zoom     | 12                 |

---

## Author

Ahmed Mohamed

---

## Tools Used

* QGIS
* XYZ Tiles Generator
* GitHub Pages

---

## License

This repository is provided for educational, research, and web mapping purposes. Please ensure compliance with the licensing terms of the original source data before redistribution or commercial use.
