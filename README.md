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

## **Implications**:
- **Seasonal Variation**: Rentals peak in warmer months, suggesting weather significantly impacts usage.
- **Hourly Influence**: Rentals are concentrated during daylight and commuting hours.
- **Usage Insights**: Data can guide operational decisions based on time of year and day.

![image](https://github.com/user-attachments/assets/961e6e71-a8d1-4d3d-b58f-75fa155de76b)
## Key Observations:
- **Right-Skewed Distribution**: Most bike rentals are low, with fewer instances of high rentals
- **Peak at Low Rentals**: The highest frequency of rentals occurs at lower counts (under 500).
- **Gradual Decrease**: Rental frequency decreases as the count increases, indicating that high rentals are uncommon.
- **Long Tail**: Occasional high demand or events leading to a surge in bike rentals
- **Small Secondary Peaks**: These may indicate specific factors or events causing higher rentals

## Implications:
- **Optimize Resources**: Focus on managing common low rentals, with readiness for occasional spikes.
- **Further Analysis**: Investigate conditions leading to smaller peaks and high rentals.

![image](https://github.com/user-attachments/assets/6018e7cc-3d4e-4886-b547-497f8a65778c)
**Key Observations**:
- **Winter**:
  - **Low Rentals**: Bike rentals are generally low, even at higher winter temperatures.
  - **Minimal Variation**: There is little variation in rentals as temperatures fluctuate, indicating that cold weather significantly suppresses bike usage.
- **Spring**:
   - **Positive Correlation**: Rentals increase as temperatures rise, indicating that warmer spring temperatures encourage more bike usage.
   - **Wider Spread**: A broader range of rentals is observed, especially at temperatures above 10°C.
- **Summer**:
   - **Strong Positive Correlation**: There is a strong increase in bike rentals as temperatures rise, with a clear peak in the range of 20°C to 30°C.
   - **High Activity**: This season shows the highest rental counts, reflecting the favorable conditions for biking.
- **Autumn**:
   - **Moderate Positive Correlation**: Similar to spring, there is a positive correlation between temperature and rentals, though the overall rental counts are slightly lower than in summer.
   - **Milder Temperatures**: The rentals remain relatively high even as temperatures drop towards the end of the season.

## Implications:
- **Seasonal Influence**: Seasonality plays a significant role in bike rental behavior, with winter showing suppressed rentals regardless of temperature, while spring, summer, and autumn show a clear positive correlation between temperature and bike usage.
 - **Operational Planning**: The data suggests that bike-sharing operations should focus on increasing availability and maintenance efforts during the warmer months, particularly in summer, where demand peaks.
- **Marketing Strategies**: Promotional efforts to encourage bike rentals could be targeted more heavily in spring and autumn, where there is a clear increase in rentals as temperatures rise.
- **Winter Considerations**: The low rentals in winter indicate that other factors (e.g., promotions, alternative incentives) may be needed to boost usage during this season, or resources could be optimized elsewhere.

