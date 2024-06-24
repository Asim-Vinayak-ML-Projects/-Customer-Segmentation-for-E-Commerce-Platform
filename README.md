# Weather Data Analysis

## Overview
This project involves analyzing weather data to understand patterns and trends using K-means clustering and parallel coordinate plots. The dataset used for this project is the `minute_weather.csv`. We performed clustering on the weather data and visualized the clusters using parallel coordinate plots.

## Dataset
The dataset contains the following columns:
- **air_pressure**: Atmospheric pressure
- **air_temp**: Air temperature
- **avg_wind_direction**: Average wind direction
- **avg_wind_speed**: Average wind speed
- **max_wind_direction**: Maximum wind direction
- **max_wind_speed**: Maximum wind speed
- **relative_humidity**: Relative humidity

## Clustering and Visualization
We used the K-means clustering algorithm to identify patterns in the weather data. The data was standardized before applying the clustering algorithm.

### Parallel Coordinate Plots
Parallel coordinate plots were used to visualize the clusters under different conditions. Here are the visualizations:

#### Parallel Plot for Relative Humidity < -0.5
<img width="843" alt="image" src="https://github.com/Asim-Vinayak-ML-Projects/Weather-Pattern-Analysis/assets/140016882/f4370be2-4b88-47b8-945f-d9ea8e713cf4">


**Analysis**:
- The blue and red clusters show significant variation across most features, particularly in air temperature and wind speed.
- The clusters with lower relative humidity tend to have higher air temperatures and more extreme wind directions and speeds.
- This plot indicates that when relative humidity is low, other weather variables exhibit more variability.

**Reason**:
- Low relative humidity often coincides with higher temperatures and dynamic atmospheric conditions, leading to greater variability in wind patterns.

#### Parallel Plot for Air Temperature > 0.5
<img width="851" alt="image" src="https://github.com/Asim-Vinayak-ML-Projects/Weather-Pattern-Analysis/assets/140016882/46da5103-f1e4-41a4-bbc1-120f92739983">


**Analysis**:
- The blue cluster shows a pronounced increase in average wind speed and maximum wind direction.
- The green and yellow clusters maintain more stable values across different features.
- Higher air temperatures are associated with increased variability in wind-related features.

**Reason**:
- Higher air temperatures can cause stronger wind currents due to thermal gradients, which can explain the increased variability in wind-related features.

#### Parallel Plot for Relative Humidity > 0.5 and Air Temperature < 0.5
<img width="860" alt="image" src="https://github.com/Asim-Vinayak-ML-Projects/Weather-Pattern-Analysis/assets/140016882/ca336a4b-0b6c-44ae-b3d3-b06439b5933b">

**Analysis**:
- The green and yellow clusters exhibit higher air pressure and more variability in wind direction.
- The black and blue clusters show a more consistent pattern with lower average wind speeds.
- This plot demonstrates that when humidity is high and temperature is low, the weather conditions tend to stabilize, especially in terms of wind speed.

**Reason**:
- When humidity is high and temperature is low, the weather conditions tend to be more stable, leading to consistent patterns in wind speed and direction.

### Scatter Plot Visualization
#### K-means Clustering
<img width="439" alt="image" src="https://github.com/Asim-Vinayak-ML-Projects/Weather-Pattern-Analysis/assets/140016882/1a8982ee-28d5-4d04-ad65-b210e53d37d7">


**Interpretation**:
- The scatter plot shows the clustering of weather data points based on the first two principal components.
- The red crosses represent the cluster centers.
- The distribution of points around the centers indicates the effectiveness of the K-means algorithm in grouping similar weather conditions.

## Conclusion
The K-means clustering algorithm effectively identified distinct patterns in the weather data, which were visualized using parallel coordinate plots. The analysis reveals how different weather conditions vary with changes in relative humidity and air temperature. The clustering approach provides insights into the relationships between various weather parameters, aiding in better understanding and prediction of weather patterns.

## Installation and Setup
### Prerequisites
- Python 3.x
- Jupyter Notebook
- Necessary libraries: pandas, numpy, matplotlib, scikit-learn

### Setup
1. Clone the repository:
   ```bash
   git clone "https://github.com/your_username/WeatherDataAnalysis.git"
   cd WeatherDataAnalysis

2. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib scikit-learn

3. Run the Jupyter Notebook:
   ```bash
   jupyter noteboom

