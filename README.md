# Weather-and-Bike-Sharing-Demand
![image](https://github.com/user-attachments/assets/6800361c-3c47-46ac-be27-679979e1b114)

# Project Overview
In this capstone project, a Data Scientist newly hired by an AI-powered weather data analytics company is tasked with analyzing how weather affects bike-sharing demand in urban areas. The project involves collecting data from various sources, performing data wrangling and exploratory analysis using tools like SQL, Tidyverse, and ggplot2, and building predictive models with Tidymodels. Additionally, an interactive dashboard will be created using R Shiny to visualize the data and predictions.The project concludes with a comprehensive report and a presentation aimed at providing actionable insights for optimizing bike-sharing systems based on weather patterns

# Understanding the source data
- **Seoul Bike Sharing Demand Data Set**: Provides hourly bike rental counts and detailed weather conditions (temperature, humidity, wind speed, etc.). This data is used to build predictive models for estimating bike demand based on weather patterns.
- **Open Weather API Data**: Offers current and forecasted weather data for over 200,000 cities, collected from various sources including weather models, satellites, and weather stations. This data is accessed via HTTP requests in R.
- **Global Bike Sharing Systems Dataset**: An HTML table from Wikipedia listing active bike-sharing systems worldwide, allowing users to understand the global context of bike-sharing programs.
- **World Cities Data**: Contains geographical information such as the name, latitude, and longitude of major cities, which helps in location-based analysis and modeling.

# Data Collection
![data collection drawio](https://github.com/user-attachments/assets/a1a73078-8c40-44cf-89ba-93913254d365)

![image](https://github.com/user-attachments/assets/819249d8-981e-49e3-abfd-ba8310047073)

## Key Observations
- **Seasonal Patterns**: 
  - **Peak Rentals**: Significant increase in rentals from April to July, peaking in mid-summer
  - **Low Rentals**: fewer rentals during winter months(Janurary-February)
- **Hourly Trends**
  - **High Activity**: Most rentals occur late morning to early evening ( 8AM to 8PM), likely during commuting and leisure times
  - **Low activity**: Fewer rentals during early morning (before 8 AM) and late eveing (after 8 PM).
- **Desity of Points**:
  - **Summer Concetration**: Densely packed points in summer months, indicating high rental activity (June-Aug)
  - **Winter dispersion**: More scattered points in winter, reflecting lower and irregular rental patterns.
- **Potential Weekday vs. Weekend Influence**:
  - **Consistent Patterns**: Suggests possible higher rentals during weekdays, particularly in commuting hours.

**Key Findings**:
- **Seasonal Variation**: Rentals peak in warmer months, suggesting weather significantly impacts usage.
- **Hourly Influence**: Rentals are concentrated during daylight and commuting hours.
- **Usage Insights**: Data can guide operational decisions based on time of year and day.
