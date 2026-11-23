# US Population Dashboard

An interactive Streamlit dashboard of US state populations from 2010 to 2019,
built by following the [Data Professor](https://github.com/dataprofessor/population-dashboard)
dashboard tutorial during my M.S. in Analytics at Dakota State University (DSU).

## Features

- **Year and color-theme pickers** in the sidebar
- **Gains/losses:** the states with the biggest population increase and decrease
  over the previous year
- **State migration donuts:** the share of states whose population grew or
  shrank by more than 50,000
- **Choropleth map** of total population by state
- **Heatmap** of population by state and year
- **Top-states table** with progress bars

## Run it

```bash
pip install -r requirements.txt
streamlit run streamlit_app.py
```

`streamlit_app_with_css.py` is the same dashboard with extra CSS to tighten the
layout and style the metric cards. Run it with
`streamlit run streamlit_app_with_css.py`.

## Data

US Census Bureau, [state population totals 2010–2019](https://www.census.gov/data/datasets/time-series/demo/popest/2010s-state-total.html).
`data/us-population-2010-2019-reshaped.csv` is the long-format version the app
uses. `US_Population.ipynb` shows how it was reshaped from the wide table.
