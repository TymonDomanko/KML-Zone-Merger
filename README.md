# KML Zone Merger

Merge every polygon zone in a KML or KMZ file into one outline, right in your browser.

**Use it:** https://tymondomanko.github.io/KML-Zone-Merger/

## What it does

- Opens a `.kml` or `.kmz` (drag and drop or choose a file)
- Merges all polygons into a single outline, with a preview of the original zones underneath
- Shows the merged area and perimeter
- Downloads the result as `.kml`, `.kmz` or GeoJSON, ready for Google Earth or Google My Maps

Your file is processed entirely in the browser. Nothing is uploaded.

## Options

| Option | What it does |
| --- | --- |
| Close gaps up to (metres) | Zones that don't quite touch stay as separate outlines. Set this to join zones within that distance of each other. `0` merges only zones that touch or overlap. |
| Fill in holes | Removes any holes left inside the merged area. |
| Keep the original zones | Adds the original zones to the output file in a hidden folder. |
| Outline style | Line colour, line width and an optional light fill. |

Only polygons are merged. Lines and pins in the file are ignored.

## Running it yourself

It's a single `index.html` with no build step. Open it in a browser, or host it anywhere that serves static files. It loads [Turf.js](https://turfjs.org/) and [JSZip](https://stuk.github.io/jszip/) from cdnjs.

## License

MIT
