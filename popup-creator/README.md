# Pop-up Creator Tool

ArcGIS pop-up template generator that extracts fields from ArcGIS Feature Services and generates styled HTML pop-up templates.

## Features

- Fetches field metadata from ArcGIS REST services
- Filters and selects fields to include
- Groups fields into sections
- Generates HTML templates ready for ArcGIS Map Viewer or Experience Builder
- Copy to clipboard or download as HTML/TXT

## Usage

1. Open `index.html` in a browser
2. Enter an ArcGIS FeatureServer URL (e.g., `https://services.arcgis.com/.../FeatureServer/0`)
3. Click "Fetch Fields from Service"
4. Select fields to include
5. Optionally group fields
6. Generate and copy/download the HTML template

## Testing

Run tests with:
```bash
npx playwright test popup-creator/
```

## Test URL

The test suite uses:
`https://services.arcgis.com/pGfbNJoYypmNq86F/arcgis/rest/services/biomed_divisions/FeatureServer/0`

