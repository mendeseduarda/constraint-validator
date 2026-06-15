# Constraint Validator

Academic project developed to explore relational data constraints and data quality concepts.

The application loads CSV datasets into DuckDB and validates predefined constraints using SQL queries.

## Supported Concepts

* Functional Dependencies (FDs)
* Conditional Functional Dependencies (CFDs)
* Denial Constraints (DCs)

## Tech Stack

* Python
* DuckDB
* SQL
* Jupyter Notebook

## Datasets

This project uses public datasets provided by the New York City Open Data platform.

### 311 Service Requests

Source:
https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2020-to-Present/erm2-nwe9/about_data

### NYC Restaurant Inspection Results

Source:
https://data.cityofnewyork.us/Health/DOHMH-New-York-City-Restaurant-Inspection-Results/43nn-pn8j/about_data

## Data Preparation

Before running the project, download the datasets manually from the links above and save the CSV files inside the `data/` directory.

Expected structure:

```text
project/
│
├── data/
│   ├── 311_service_requests.csv
│   └── restaurant_inspections.csv
│
├── notebooks/
│   └── *.ipynb
│
├── requirements.txt
└── README.md
```

## Installation

Clone the repository:

```bash
git clone <repository-url>
cd constraint-validator
```

Create and activate a virtual environment:

### macOS / Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

Example `requirements.txt`:

```text
duckdb
pandas
jupyter
notebook
```

## Running the Project

1. Download the datasets from the provided sources.
2. Save the CSV files inside the `data/` folder.
3. Install the project dependencies.
4. Start Jupyter Notebook:

```bash
jupyter notebook
```

5. Open the notebooks in the `notebooks/` directory and execute the cells.

## Disclaimer

The datasets are not distributed with this repository. Users must obtain the latest versions directly from the official NYC Open Data portal.
