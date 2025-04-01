# Project Overview
The increasing global demand for food places immense pressure on natural resources, contributing significantly to environmental degradation. According to [Our world in Data](https://ourworldindata.org/environmental-impacts-of-food), food production accounts for 26% of global greenhouse gas emissions, occupies half of the world’s habitable land, and is responsible for 70% of freshwater withdrawals. Additionally, agricultural activities contribute to 78% of global ocean and freshwater eutrophication, leading to severe nutrient pollution in waterways.

Without intervention, these environmental impacts will continue to accelerate climate change, deplete water resources, and threaten biodiversity. Understanding the environmental footprint of different food products is crucial for designing sustainable food systems. This project aims to quantify and analyze these impacts, identifying high-impact areas and potential pathways for sustainability.

By leveraging data-driven insights, we will explore:

- The extent of greenhouse gas emissions, water consumption, and land use associated with different food types.

- The comparative impact of plant-based vs. animal-based products.

- The contribution of different foods to water pollution through eutrophication.

- Actionable strategies to promote sustainable food choices at both consumer and policy levels.

# CRISP-DM Framework Implementation

To ensure a structured and systematic analysis, this project follows the CRISP-DM (Cross Industry Standard Process for Data Mining) framework.

#  1. Business Understanding
Objectives:

* Analyze the environmental impact of food production in four key areas:

    - Carbon emissions

    - Water usage

    - Land use

    - Biodiversity loss

* Identify high-impact foods and compare plant-based vs. animal-based products.

* Provide actionable recommendations for reducing environmental impact.

# 2. Data Understanding

The [dataset](https://azubiafrica-my.sharepoint.com/:x:/r/personal/teachops_azubiafrica_org/_layouts/15/Doc.aspx?sourcedoc=%7B3E112463-368D-41C7-A8F0-A784AF801F3E%7D&file=Food_Production.csv&action=default&mobileredirect=true) contains 43 of the most common foods globally, with 23 columns detailing their respective land, water usage, and carbon footprint.

* Greenhouse Gas Emissions

    - Land use change (Kg CO₂-eq per kg product)

    - Animal Feed (Kg CO₂-eq per kg product)

    - Farm (Kg CO₂-eq per kg product)

    - Processing, Transport, Packaging, Retail emissions

* Water Usage

    - Freshwater withdrawals per kg, per 100g protein, per 1000 kcal

    - Scarcity-weighted water use (liters per kg, per 100g protein, per 1000 kcal)

* Land Use

    - Land use per kg, per 100g protein, per 1000 kcal

* Eutrophication (Nutrient Pollution Impact)

    - Eutrophying emissions per kg, per 100g protein, per 1000 kcal

# 3. Data Preparation
The dataset was imported and processed using Python, with key libraries such as pandas, NumPy, and Matplotlib for analysis and visualization. Initial exploration involved fundamental checks - .head(), .tail(), and .shape()-revealing 43 rows (food items) and 23 columns (environmental metrics). There were no duplicate entries, but missing values were present across several columns.

* Outliers Analysis
  
As part of our exploratory data analysis, we identified several outliers, which revealed skewness in our data. This step was crucial, as outliers can distort statistical analyses and lead to misleading conclusions. It helped guide our approach to handling missing values and informed our decisions about the imputation methods we would apply later on.

* Correlation Analysis

    - Strong Positive Correlations

    Greenhouse gas emissions per 100g protein strongly correlate with land use change (~0.86), emphasizing that land-intensive food production significantly drives emissions.

    Land use per kilogram is highly correlated with land use per 100g protein (~0.91), showing that land requirements scale with protein content.

    Total emissions and farm emissions have a high correlation, confirming that farm-level activities dominate the environmental footprint.

    - Moderate Correlstion

    Scarcity-weighted water use per kg moderately correlates with land use (~0.59), implying that resource-heavy foods demand both land and water.

    - Weak or No Correlation
    
    Transport emissions show minimal correlation with most variables, reinforcing that food production has a far greater impact than transportation in environmental costs.

    Eutrophication emissions per kilogram negatively correlate with some land and water metrics, suggesting nutrient pollution doesn’t always scale with resource use.

# 4. Modeling

# 5. Evaluation

# 6. Deployment

 Tools Used



