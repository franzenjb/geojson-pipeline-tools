# Create GeoJSON Tool

CSV to GeoJSON converter - transforms CSV data into GeoJSON files at multiple geographic levels.

## Features

- Upload CSV files with geographic identifiers
- Support for ZIP codes, FIPS codes, ECODE/RCODE/DCODE
- Create GeoJSON at multiple levels: ZIP, County, Chapter, Region, Division
- Automatic data aggregation (count or sum)
- Progress tracking during generation
- Direct download of resulting GeoJSON

## Supported Geographic Levels

| Level | Identifier | Description |
|-------|------------|-------------|
| ZIP | 5-digit ZIP code | US ZIP Code Tabulation Areas |
| County | FIPS code | US Counties (3,143 features) |
| Chapter | ECODE | Red Cross Chapters (226 features) |
| Region | RCODE | Red Cross Regions (48 features) |
| Division | DCODE | Red Cross Divisions (6 features) |

## Data Sources

Boundary files are loaded from [red-cross-data](https://github.com/franzenjb/red-cross-data):
- `us_zctas.json` - ZIP Code boundaries
- `arc_counties.geojson` - County boundaries with Red Cross codes
- `arc_chapters.geojson` - Chapter boundaries
- `arc_regions.geojson` - Region boundaries
- `arc_divisions.geojson` - Division boundaries

## Usage

1. Open `index.html` in a browser
2. Upload a CSV file with geographic identifiers
3. Select the column containing your geographic codes
4. Choose the output geographic level
5. Optionally select a value column to aggregate
6. Click Generate to create your GeoJSON
7. Download the result for use in ArcGIS, QGIS, or web maps
