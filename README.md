## Python API Challenge


# Overview
The Python API Challenge explores the relationship between weather conditions and geographical location, with a particular focus on latitude. Through two major parts—WeatherPy and VacationPy—this project uses APIs to retrieve, analyze, and visualize weather data, and to identify ideal vacation destinations based on specific weather conditions.

This project demonstrates the use of Python for data analysis, visualization, and API interaction, providing insights into the weather as we approach the equator.

File Structure
WeatherPy.ipynb:

Analyzes weather data from over 500 randomly selected cities using the OpenWeatherMap API.
Includes scatter plots showing the relationships between latitude and various weather parameters.
Performs linear regression to study weather patterns in the Northern and Southern Hemispheres.

-- VacationPy.ipynb:

Uses weather data to identify cities that meet specific weather conditions for ideal vacations.
Employs the Geoapify API to locate hotels near selected cities and displays an interactive map with hover information.

-- .gitignore:

Excludes sensitive files such as api_keys.py to prevent accidental exposure of API keys.

-- api_keys.py:

Contains the API keys for OpenWeatherMap and Geoapify APIs (excluded from GitHub for security).

## Part 1: WeatherPy
Objectives

# Visualize Weather Across Cities:

Retrieve weather data for 500+ cities using the OpenWeatherMap API.
Generate scatter plots to study the relationships between latitude and:
Temperature
Humidity
Cloudiness
Wind Speed

# Compute Linear Regression:

Analyze weather patterns in the Northern and Southern Hemispheres.
Create regression plots with:
Linear regression lines
Model formulas
R² values
Key Outputs
Scatter plots of latitude vs. weather parameters.
Linear regression plots for Northern and Southern Hemispheres for each parameter.


## Part 2: VacationPy
## Objectives

# Identify Ideal Vacation Cities:

Filter cities based on custom weather conditions (e.g., temperature, cloudiness, wind speed).
Create a narrowed-down DataFrame of ideal cities.

# Locate Nearby Hotels:

Use the Geoapify API to find the nearest hotel within 10,000 meters of each selected city.
Add hotel names and countries to the data.

# Visualize Data:

Display an interactive map with points representing cities.
Include hover functionality showing city, country, and hotel name.

# Key Outputs
An interactive map displaying selected vacation cities and nearby hotels.

## Technologies and Tools Used
Python Libraries:
pandas: Data manipulation.
matplotlib: Visualization.
requests: API interaction.
numpy: Statistical computations.
scipy.stats: Linear regression.
hvplot and geoviews: Interactive geographic visualizations.


## APIs:
OpenWeatherMap API: Weather data retrieval.
Geoapify API: Hotel location services.


## How to Run the Project
Prerequisites
--Clone the repository:
git clone https://github.com/<your-username>/python-api-challenge.git
cd python-api-challenge

--Install dependencies:
pip install -r requirements.txt


--Add API keys:

Save your OpenWeatherMap and Geoapify API keys in a file named api_keys.py with the following format:
   weather_api_key = "your_openweathermap_api_key"
   geoapify_key = "your_geoapify_api_key"

## Steps
Open the notebooks:
jupyter notebook
Run the WeatherPy.ipynb notebook:
Generate scatter plots and linear regression models for weather variables.
Run the VacationPy.ipynb notebook:
Filter cities based on ideal weather conditions.
Create an interactive map of vacation destinations.

## Results and Insights

--WeatherPy
Temperature vs. Latitude: Confirms that temperatures increase as you approach the equator.
Humidity vs. Latitude: No consistent trend observed.
Cloudiness vs. Latitude: Patterns vary with latitude but do not show a strong correlation.
Wind Speed vs. Latitude: No clear relationship identified.

--VacationPy
Ideal Vacation Cities: Identified cities with comfortable weather conditions.
Hotel Map: Interactive visualization showing hotels near selected cities.
Project Requirements

--WeatherPy
Scatter plots for:
Latitude vs. Temperature
Latitude vs. Humidity
Latitude vs. Cloudiness
Latitude vs. Wind Speed
Linear regression for:
Northern and Southern Hemispheres.

--VacationPy
Filter cities based on custom weather conditions.
Locate hotels near cities using Geoapify API.
Interactive map displaying cities, hotels, and hover details.

## Challenges and Learning

--This project involved:

Working with APIs and JSON responses.
Handling geographic data and visualizing it with maps.
Developing custom filtering logic for vacation planning.
Managing Git repositories and excluding sensitive data.
