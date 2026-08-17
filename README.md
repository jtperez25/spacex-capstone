# SpaceX Falcon 9 First Stage Landing Prediction

**IBM Data Science Professional Certificate — Applied Data Science Capstone**

## Overview

SpaceX advertises Falcon 9 rocket launches at a cost of $62 million, compared to other providers who charge upward of $165 million per launch. Much of this savings comes from SpaceX's ability to reuse the first stage of the rocket. This project builds a data science pipeline to predict whether the Falcon 9 first stage will successfully land, which can help estimate launch costs and inform competitive bidding decisions.

The project covers the full data science workflow: data collection, wrangling, exploratory data analysis, interactive visualization, and predictive modeling using classification algorithms.

## Project Structure

| File | Description |
|---|---|
| `JoshuaPerez_jupyter-labs-spacex-data-collection-api_completed.ipynb` | Collects launch data via the SpaceX REST API |
| `JoshuaPerez_jupyter-labs-webscraping_completed.ipynb` | Scrapes Falcon 9/Heavy launch records from Wikipedia |
| `JoshuaPerez_labs-jupyter-spacex-Data_wrangling_completed.ipynb` | Cleans data and engineers the binary landing-outcome label |
| `JoshuaPerez_eda-with-visualization-lab_completed.ipynb` | Exploratory data analysis using matplotlib/seaborn |
| `JoshuaPerez_jupyter-labs-eda-sql-coursera_sqllite_completed.ipynb` | Exploratory data analysis using SQL queries |
| `JoshuaPerez_lab_jupyter_launch_site_location_completed.ipynb` | Interactive launch site mapping with Folium |
| `spacex-dash-app.py` | Interactive Plotly Dash dashboard for launch records |
| `JoshuaPerez_SpaceX_Machine_Learning_Prediction_Part_5_completed.ipynb` | Trains and evaluates classification models to predict landing success |

## Methodology

1. **Data Collection** — Launch records gathered from the SpaceX API and Wikipedia via web scraping.
2. **Data Wrangling** — Missing values handled, categorical outcomes converted into a binary `Class` label (1 = successful landing, 0 = unsuccessful).
3. **Exploratory Data Analysis** — Relationships between payload mass, launch site, orbit type, and landing success examined via both SQL queries and visualizations.
4. **Interactive Visual Analytics** — Launch sites mapped geospatially with Folium; an interactive Dash dashboard built to explore success rates by site and payload range.
5. **Predictive Analysis** — Logistic Regression, SVM, Decision Tree, and KNN classifiers trained and tuned via `GridSearchCV`; models compared on test accuracy to identify the best-performing algorithm.

## Key Findings

- **KSC LC-39A** has both the most successful launches (10) and the highest success rate (76.9%) among all launch sites.
- Payload masses in the **2,000–4,000 kg** range have the highest landing success rate (61.9%), while the **6,000–8,000 kg** range has the lowest (0%).
- The **B5** booster version achieved a 100% success rate, followed by **FT** at 66.7%.

## Tools & Technologies

Python · Pandas · NumPy · Scikit-learn · SQL (SQLite) · Folium · Plotly · Dash · Matplotlib · Seaborn

## Author

Joshua Perez
