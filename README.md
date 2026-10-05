# COVID-19 Global Dashboard (Tableau)

An interactive Tableau dashboard that summarises the global impact of COVID-19: how many people were infected, how many died, which regions and countries were hit hardest, and how infection rates are projected to change.

**Live dashboard:** [Add your Tableau Public link here]

![Dashboard preview](dashboard.png)


---

## Project Overview

This project takes raw COVID-19 case and death data, cleans and prepares it, and turns it into a single-page dashboard that answers four questions:

1. How big was the pandemic globally?
2. Which continents recorded the most deaths?
3. Which countries had the highest share of their population infected?
4. How did infection rates change over time, and where are they heading?

The data covers the period from **late 2019 to 30 April 2021**.

---

## What the Dashboard Shows

### 1. Global Numbers
A summary table of the headline figures:

| Metric | Value |
|---|---|
| Total Cases | 150,574,977 |
| Total Deaths | 3,180,206 |
| Death Percentage | 2.11% |

The death percentage is calculated as `Total Deaths / Total Cases x 100`. Roughly 2 in every 100 confirmed cases ended in death.

### 2. Total Deaths Per Continent
A bar chart ranking continents by total death count.

- **Europe** has the highest number of deaths (about 1 million), followed by **North America**, **South America** and **Asia**.
- **Africa** and **Oceania** recorded far fewer deaths.
- Note that these are raw counts, not rates, so population size and testing levels also influence the ranking.

### 3. Percent Population Infected Per Country
A world map where each country is shaded by the percentage of its population that has been infected. Darker red means a higher infection rate, and the colour scale runs from **0% to 17.13%**.

- Countries in **Europe** and the **Americas** (including the United States) show the darkest shading.
- Much of **Africa** and **Asia** appears lighter, though low reported infection rates can reflect limited testing rather than fewer infections.
- Countries with no matching data are counted as "unknown" in the bottom corner of the map.

### 4. Percent Population Infected Over Time (with Forecast)
A line chart tracking the average percent of the population infected by month for five countries: **China, India, Mexico, the United Kingdom and the United States**.

- **Solid lines** show actual recorded data.
- **Lighter lines with shaded bands** show Tableau's forecast, with the shaded area representing the prediction interval (the range of likely values).
- Highlighted data labels show the latest values, for example the **United States at 8.35%** and **Mexico at 0.56%** at the end of the actual data.
- The forecast projects the United States continuing to climb, while China and India stay comparatively low.

---

## Tools and Skills Used

- **Tableau** for building the worksheets and the final dashboard
- **Microsoft Excel** as the data source (85,171 rows)
- **Calculated fields** (e.g. Death Percentage, Percent Population Infected)
- **Data type fixes** to convert text values (comma decimals) into numeric measures
- **Geographic mapping** using Tableau's built-in geocoding and background layers
- **Time-series forecasting** using Tableau's forecast feature
- **Dashboard design**: layout, colour scales, titles and number formatting

---

## Data

- **Source:** COVID-19 case and death data (Our World in Data / publicly available global COVID-19 dataset)
- **Fields used:** Location, Continent, Date, Population, Total Cases, Total Deaths, Highest Infection Count, Percent Population Infected
- **Time range:** up to 30 April 2021

---

## How to Use the Dashboard

1. Open the live Tableau Public link above.
2. Hover over any bar, country or line to see exact values in the tooltip.
3. Use the legend on the right of the line chart to identify each country and whether the line is actual or estimated.

To open the workbook locally, download the `.twbx` file from this repository and open it in Tableau Public or Tableau Desktop.

---

## Key Takeaways

- Over **150 million** cases and **3.18 million** deaths were recorded globally by the end of April 2021.
- **Europe** had the highest total deaths of any continent.
- The **United States** had the highest percentage of its population infected among the countries tracked, and the forecast suggested it would keep rising.
- Raw counts and percentages tell different stories, so using both gives a fuller picture.

---

