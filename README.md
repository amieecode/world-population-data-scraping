# world-population-data-scraping
## About Dataset
*Context:*
This dataset provides a snapshot of world population estimates for the year 2026, including demographic, geographic, and urbanization data. It covers 233 countries and territories and includes key metrics such as population, population density, fertility rate, median age, urban population %, net migration, and share of the world population.

The dataset is useful for educational, research, and analytical purposes, helping data enthusiasts, students, and businesses explore global population trends.

*Data Description:*
- Rank – Country rank by population
- Country – Name of the country or dependency
- Population_2026 – Estimated population in 2026
- Yearly_Change – % change in population from the previous year
- Net_Change – Absolute change in population
- Density_per_km2 – Population per square kilometer
- Land_Area_km2 – Total land area in km²
- Migrants_Net – Net migration (people moving in/out)
- Fertility_Rate – Average number of children per woman
- Median_Age – Median age of the population
- Urban_Population_pct – % of population living in urban areas
- World_Share_pct – % of world population represented by this country

*Source / Provenance:*
- Data was collected from Worldometer (https://www.worldometers.info/world-population/population-by-country/).
- It is publicly available for educational and research purposes.

*Collection Methodology:*
1) Web Scraping: Extracted using Python’s pandas.read_html() function from the Worldometer website.

2) Data Cleaning & Transformation:
    - Percentages converted to floats (Yearly Change, Urban Population %, World Share %).
    - Impossible zeros (e.g., Fertility Rate, Median Age) were replaced with median or verified real values.
    - Density was recalculated only when Land Area values were corrected.
    - Numeric columns were converted to correct types (int or float) for analysis.
3) Final Dataset: Contains clean, ready-to-use data for 233 countries/territories with demographic and population metrics.

Acknowledgement:

World Population | Worldometer
