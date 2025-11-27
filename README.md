# GeoJSON Pipeline Tools

A collection of independent ArcGIS and geospatial tools, each in its own directory. Each tool is completely self-contained and can be developed, tested, and deployed independently.

## 🎯 Philosophy

**Each tab = One tool = One directory = One project**

This repository keeps tools organized separately so they don't get "marbled together." Each tool:
- Has its own directory
- Is self-contained (no shared dependencies)
- Can be developed independently
- Has its own tests
- Can be deployed separately

## 📁 Structure

```
geojson-pipeline-tools/
├── popup-creator/        ✅ Ready - ArcGIS pop-up template generator
├── geocoder/             ✅ Ready - MapBox geocoding with batch CSV support
├── code-lookup/          ✅ Ready - Red Cross code lookup tool
├── create-geojson/       ✅ Ready - CSV to GeoJSON converter
└── orgler-creator/       ✅ Ready - Power BI to Orgler converter
```

## 🌐 Live Demo

**Access the tools online**: [https://franzenjb.github.io/geojson-pipeline-tools/](https://franzenjb.github.io/geojson-pipeline-tools/)

## 🚀 Quick Start

1. **View all tools**: Open `index.html` in a browser or visit the [live demo](https://franzenjb.github.io/geojson-pipeline-tools/)
2. **Use a tool**: Navigate to any tool's directory and open its `index.html`
3. **Run tests**: `npm test` (runs all) or `npm run test:popup` (specific tool)

## 🛠️ Development

Each tool directory contains:
- `index.html` - The tool itself
- `README.md` - Tool-specific documentation
- `package.json` - Tool metadata (optional)
- `test-*.spec.js` - Playwright test suite (if applicable)

## ✅ Current Status

All 5 tools are now complete and ready to use:

- **Pop-up Creator**: ✅ Complete - ArcGIS pop-up template generator with Playwright tests
- **Geocoder**: ✅ Complete - MapBox geocoding with single address and batch CSV support
- **Code Lookup**: ✅ Complete - Search 33,000+ ZIP codes for Red Cross codes (ECODE, RCODE, DCODE, FIPS)
- **Create GeoJSON**: ✅ Complete - Transform CSV data to GeoJSON at ZIP/County/Chapter/Region/Division levels
- **Orgler Creator**: ✅ Complete - Convert Power BI URLs to Story Map and RCView embed formats

## 📝 Testing

Run all tests:
```bash
npm test
```

Run tests for a specific tool:
```bash
npx playwright test popup-creator/
```

## 🚀 Deployment

This repository is automatically deployed to GitHub Pages via GitHub Actions.

**To deploy:**
1. Push changes to the `main` branch
2. GitHub Actions will automatically build and deploy to GitHub Pages
3. The site will be available at `https://franzenjb.github.io/geojson-pipeline-tools/`

**Manual deployment** (if needed):
- Go to repository Settings → Pages
- Source: GitHub Actions
- The workflow (`.github/workflows/deploy.yml`) handles deployment automatically

## 🎨 Why This Structure?

This structure ensures:
- ✅ **Separation of concerns** - Each tool is independent
- ✅ **Easy maintenance** - Changes to one tool don't affect others
- ✅ **Clear organization** - Easy to find and work on specific tools
- ✅ **Independent deployment** - Deploy tools separately if needed
- ✅ **No file conflicts** - Each tool has its own namespace
- ✅ **Web-accessible** - All tools work in any modern browser, no server required

