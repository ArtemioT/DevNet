# DevNet

A real estate agent search website that allows users to search for realtors, view their information, and save results as a PDF.

## Pages

- **Home** (`index.html`) — Search bar to look up realtors with autocomplete, with an option to save results as a PDF
- **List** (`list.html`) — Full table view of all realtors
- **About Us** (`aboutus.html`) — Info about the team (3 freshmen, 1 sophomore)
- **The Code** (`ourcode.html`) — Screenshots of the Python scraper and JavaScript search bar code

## Features

- Autocomplete search for realtors
- PDF export of search results using jsPDF
- Python web scraper to extract realtor data and export to CSV

## Scraper

`scraper.py` fetches realtor data from the live site, parses the embedded JSON, sorts realtors alphabetically by name, and writes the results to `realtors.csv`.

**Dependencies:** `requests`, `beautifulsoup4`

```bash
pip install requests beautifulsoup4
python scraper.py
```

## Tech Stack

- HTML, CSS, JavaScript (frontend)
- Python (web scraping)
- jsPDF (PDF generation)
