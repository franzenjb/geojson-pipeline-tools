# MapBox Geocoding Tool

Convert addresses to coordinates using the MapBox Geocoding API.

## Features

- **Single Address Geocoding**: Geocode individual addresses with instant results
- **Batch CSV Processing**: Upload CSV files with addresses and geocode them in bulk
- **Interactive Map**: Visualize geocoded results on an interactive MapBox map
- **Progress Tracking**: Real-time progress bar and status updates for batch operations
- **Results Export**: Download geocoded results as CSV files
- **Local Storage**: API key stored securely in browser localStorage

## MapBox API

- **Free Tier**: 100,000 geocodes per month
- **Get API Key**: [mapbox.com/access-tokens](https://account.mapbox.com/access-tokens/)
- **Rate Limit**: 600 requests per minute

## Usage

1. Enter your MapBox API key (starts with `pk.`)
2. Choose single address or CSV batch geocoding
3. View results in the table and on the interactive map
4. Download results as CSV

## CSV Format

Your CSV file should have an "address" column (case-insensitive). The tool will:
- Preserve all original columns
- Add latitude, longitude, place_name, and confidence columns
- Handle CSV files with quoted fields

## Browser Compatibility

Works in all modern browsers. Requires JavaScript enabled.

