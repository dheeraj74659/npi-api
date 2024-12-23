# NPI Data Fetcher

This Python script fetches data from the [NPI Registry](https://npiregistry.cms.hhs.gov/) for a list of NPI numbers, processes the data, and outputs the results in a structured format (Pandas DataFrame). The script performs the following tasks:
- Reads a list of NPI numbers from a CSV file.
- Fetches data from the NPI Registry API for each NPI number.
- Extracts key information (basic details, addresses, and specialties) for each NPI.
- Saves the results into a DataFrame for further analysis or export.

## Features

- Fetches basic provider information (name, credentials, last updated).
- Extracts mailing and physical addresses.
- Extracts primary and secondary specialties (taxonomy).
- Handles missing data and errors gracefully with logging and retry mechanisms.
- Outputs the results as a Pandas DataFrame.

## Requirements

- Python 3.x
- `requests` library for making HTTP requests to the NPI Registry API.
- `pandas` library for data manipulation.

You can install the required libraries using `pip`:

```bash
pip install -r requirements.txt
