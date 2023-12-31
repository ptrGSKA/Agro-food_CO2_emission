# Agro-food_CO2_emission
About Dataset

The agricultural CO2 emission dataset has been constructed by merging and reprocessing approximately a dozen individual datasets from the Food and Agriculture Organization (FAO) and data from IPCC. These datasets were, cleaned, preprocessed and merged together to create a comprehensive and cohesive dataset for analysis and forecasting purposes.

The dataset, as demonstrated in the notebook, describes CO2 emissions related to agri-food, which amount to approximately 18.5% of the global annual emissions.

Indeed, the emissions from the agri-food sector are significant when studying climate change. As the dataset shows, these emissions contribute to a substantial portion of the global annual emissions. Understanding and addressing the environmental impact of the agri-food industry is crucial for mitigating climate change and developing sustainable practices within this sector.

For a better understanding of the dataset, I have written a notebook where I perform an analysis of the relationship between emissions, climate change and geografic Area.
Additionally, I provide an example of regression to predict the percentage variations in temperatures.

<p></p>
<p align="center">
<img src= "Emissions-by-sector-pie-charts.png" width=600>
</p>

Source: Climate Watch, the World Resources Institute via OurWorldinData.org. Licensed under Creative Commons by author Hannah Richie (2020)

# Description

The primary goal of this project is to analyze the impact of CO2 emissions on the agricultural sector, identify regions that stand out from the rest, and create an ARIMA model to predict short-term temperature fluctuations in a specific geographical area.

The project comprises numerous visual representations that facilitate the comparison of different regions and enable the observation of the correlation between emitters.

Despite the pre-cleaning of the data, numerous missing values still exist. These values, lacking source information, will be considered as zero, potentially introducing bias into the analysis.

- Given the self-explanatory nature of the data, extensive exploratory data analysis (EDA) is not required, as the visualization will effectively convey the information.
- Next the handling of the missing values to the fullest extent possible.
- During the feature engineering phase, two additional features are incorporated, specifically the continent and world region in which the country is situated. These newly introduced features will prove beneficial in the subsequent analysis and visualization processes.
- Moving forward, the data visualization stage where the dataset undergoes visualization, enabling the exploration of several significant aspects of the data.
Followed by regional emissions and emissions by capita
- Following the examination of potential correlations between regions, proceeded to carry out a series of statistical tests to determine the significance of these relationships.
- The final stage involves the creation of an ARIMA model, which is utilized to generate short-term predictions for Europe and Asia regions.

## Objectives

- Is there a direct correlation between emission, population growth and temperature increase?
- Which are the most and least polluting countries?
- How do the certain regions contribute to the emissions?
- Which regions are the most effected ones?
- What are the emissions per capita in the different regions, which region pollutes the most?
- Which countries are with the least emissions due to Forestland and what is their correlation with their total emission and population?
- Is the emission difference between regions significant?
- What are the predictions for the next few years/decade?

## Dataset Features:

    - Savanna fires: Emissions from fires in savanna ecosystems.
    - Forest fires: Emissions from fires in forested areas.
    - Crop Residues: Emissions from burning or decomposing leftover plant material after crop harvesting.
    - Rice Cultivation: Emissions from methane released during rice cultivation.
    - Drained organic soils (CO2): Emissions from carbon dioxide released when draining organic soils.
    - Pesticides Manufacturing: Emissions from the production of pesticides.
    - Food Transport: Emissions from transporting food products.
    - Forestland: Land covered by forests.
    - Net Forest conversion: Change in forest area due to deforestation and afforestation.
    - Food Household Consumption: Emissions from food consumption at the household level.
    - Food Retail: Emissions from the operation of retail establishments selling food.
    - On-farm Electricity Use: Electricity consumption on farms.
    - Food Packaging: Emissions from the production and disposal of food packaging materials.
    - Agrifood Systems Waste Disposal: Emissions from waste disposal in the agrifood system.
    - Food Processing: Emissions from processing food products.
    - Fertilizers Manufacturing: Emissions from the production of fertilizers.
    - IPPU: Emissions from industrial processes and product use.
    - Manure applied to Soils: Emissions from applying animal manure to agricultural soils.
    - Manure left on Pasture: Emissions from animal manure on pasture or grazing land.
    - Manure Management: Emissions from managing and treating animal manure.
    - Fires in organic soils: Emissions from fires in organic soils.
    - Fires in humid tropical forests: Emissions from fires in humid tropical forests.
    - On-farm energy use: Energy consumption on farms.
    - Rural population: Number of people living in rural areas.
    - Urban population: Number of people living in urban areas.
    - Total Population - Male: Total number of male individuals in the population.
    - Total Population - Female: Total number of female individuals in the population.
    - total_emission: Total greenhouse gas emissions from various sources.
    - Average Temperature °C: The average increasing of temperature (by year) in degrees Celsius

Importance and Context:

The agricultural sector contributes to approximately, how i'll demostrate in my notebook, 62% of the total global CO2 emissions, making it a significant contributor to climate change. This dataset plays a crucial role in understanding and monitoring the impact of agricultural activities on CO2 emissions. By leveraging machine learning techniques, it enables the forecasting of future emissions, allowing policymakers and researchers to develop targeted strategies and interventions for sustainable agricultural practices. This dataset serves as a valuable resource for climate scientists, environmental researchers, and policymakers striving to mitigate the environmental impact of the agricultural sector.

Note:

    CO2 is recorded in kilotons (kt): 1 kt represents 1000 kg of CO2.
    The feature "Average Temperature C°", which can be used as the target for machine learning models, represents the average yearly temperature increase. For example, if it is 0.12, it means that the temperature in that specific location increased by 0.12 degrees Celsius.
    Forestland is the only feature that exhibits negative emissions due to its role as a carbon sink. Through photosynthesis, forests absorb and store carbon dioxide, effectively removing it from the atmosphere. Sustainable forest management, along with afforestation and reforestation efforts, further contribute to negative emissions by increasing carbon sequestration capacity.
    If you prefer Fahrenheit to Celsius, here is the formula: °F = (°C x 9/5) + 32
