# Orgler Creator Tool

Convert Power BI URLs to embed formats for Story Maps and RCView dashboards.

## Features

- Parse Power BI report URLs (public embed, report links, embed links)
- Generate embed codes for multiple platforms:
  - ArcGIS StoryMaps
  - RCView Dashboards
  - Standard HTML iframe
- Configurable embed options:
  - Hide/show navigation pane
  - Hide/show filter pane
  - Transparent background
  - Custom width and height
- One-click copy to clipboard
- URL testing (opens in new tab)

## Supported URL Formats

1. **Public Embed URL**: `https://app.powerbi.com/view?r=eyJ...`
2. **Report Link**: `https://app.powerbi.com/groups/.../reports/...`
3. **Embed Link**: `https://app.powerbi.com/reportEmbed?reportId=...`

## Usage

1. Open `index.html` in a browser
2. Copy your Power BI report URL (from "Publish to web" or sharing)
3. Paste it into the input field
4. Adjust embed options as needed
5. Click "Generate Embed Codes"
6. Copy the appropriate format for your target platform

## Platform Notes

- **Story Map**: Use in ArcGIS StoryMaps "Embed" block
- **RCView**: Use in RCView Dashboard iframe widgets
- **HTML iframe**: Use in any website or web application
