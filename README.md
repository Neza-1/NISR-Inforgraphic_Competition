# Rwanda Seasonal Agricultural Survey 2025 Dashboard

An interactive Streamlit dashboard exploring Rwanda’s 2025 Seasonal Agricultural Survey. The project visualizes agricultural land use, crop production, farm practices, harvest allocation, economic value, and official NISR survey tables.

## Live Demo

Explore the deployed dashboard: [https://vincent-nisr-inforgraphiccompetition.streamlit.app/](https://vincent-nisr-inforgraphiccompetition.streamlit.app/)

## Features

- **Data Story:** Five narrative chapters covering land use, inputs, crop output, harvest allocation, and gross value added.
- **Infographic Poster:** A responsive visual summary of key 2025 agricultural indicators.
- **Simulator & District Explorer:** Explore district-level land profiles and estimate harvest allocations.
- **Survey Tables:** Search, filter, chart, and export the official SAS 2025 tables.
- **Interactive Visualizations:** Plotly charts and responsive Streamlit components.

## Technology

- Python
- Streamlit
- Pandas
- NumPy
- Plotly
- OpenPyXL
- Excel workbook data

## Getting Started

### Prerequisites

- Python 3.10 or newer
- pip

### Installation

```bash
git clone https://github.com/Neza-1/NISR-Inforgraphic_Competition.git
cd NISR-Inforgraphic_Competition
python -m venv .venv
```

Activate the virtual environment:

```bash
# Linux/macOS
source .venv/bin/activate

# Windows
.venv\Scripts\activate
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

### Run the Dashboard

```bash
streamlit run app.py
```

The application opens in your browser at:

```text
http://localhost:8501
```

## Data

The dashboard reads:

```text
SAS 2025_Annual Tables.xlsx
```

The workbook contains the official NISR Seasonal Agricultural Survey tables, including:

- National summary indicators
- Gross value added
- Harvest allocation
- District agricultural land use
- Land cover
- Farm inputs
- Crop production and yield
- Irrigation and conservation practices

The application caches loaded datasets with Streamlit’s `@st.cache_data` decorator for faster interactions.

## Dashboard Views

### 1. Data Story

Presents an interactive narrative covering:

- Agricultural land and spatial distribution
- Soil protection and farm inputs
- Production of major crops
- Harvest sales versus household consumption
- Gross value added per hectare

### 2. Infographic Poster

Displays a printable-style summary of major indicators for Rwanda’s agricultural sector.

### 3. Simulator & Districts

Allows users to:

- Estimate sales, home use, seed, gifts, and losses for a selected harvest
- Explore land-use indicators across Rwanda’s 30 districts
- Compare cultivated land, pasture, seasonal crops, and permanent crops

### 4. Survey Tables

Provides access to the 79 official survey tables.

Users can:

- Browse tables by thematic category
- Search records
- Select visible columns
- Generate quick charts
- Download filtered results as CSV

## Key Indicators

- 59.9% of national land used for agriculture
- 1.42 million hectares of agricultural land
- 90.3% of plots protected with terraces or trenches
- 88.0% organic manure use
- 63.2% mineral fertilizer use
- 58.9% Season C irrigation use

## Source

- National Institute of Statistics of Rwanda
- Seasonal Agricultural Survey 2025 Annual Report

Data source: `SAS 2025_Annual Tables.xlsx`

## Competition

This application was developed for the 2026 NISR Infographic Competition under the theme:

**“Feeding the Land of a Thousand Hills”**
