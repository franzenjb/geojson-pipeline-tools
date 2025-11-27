# Code Lookup Tool

Red Cross code lookup tool - search by name to find ECODE, RCODE, DCODE, and FIPS codes.

## Features

- Search Red Cross chapters, regions, divisions, and counties
- Find ECODE, RCODE, DCODE, and FIPS codes
- 33,000+ ZIP code records with full organizational mapping
- Real-time search with filtering by field type
- Database statistics display

## Data Source

Data is loaded from the [red-cross-data](https://github.com/franzenjb/red-cross-data) repository:
- `lookup_database.json` - Chapter and county lookup data
- `zip_to_redcross.csv` - Complete ZIP to Red Cross mapping

## Usage

1. Open `index.html` in a browser
2. Wait for the database to load (33,000+ records)
3. Select a search type (All Fields, Chapter, Region, etc.)
4. Enter your search term
5. View results with all associated codes

## Code Reference

- **ECODE** - Entity Code: Unique identifier for each Red Cross chapter
- **RCODE** - Region Code: Identifies the region (e.g., 17R08)
- **DCODE** - Division Code: Identifies the division (e.g., D24)
- **FIPS** - Federal Information Processing Standard code for counties
