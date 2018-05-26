# What's the Weather Like? 

By *Aidin Hassanzadeh*
___

This repository contains Python/IPython files for the 'What's the Weather Like?' project.
The aim of this project is to perform quantitative analysis of different weather trend data with respect to latitude.
This project follows the below 6 objectives:

- Demonstrate and analyse Temperature variations (F) vs. Latitude
- Demonstrate and analyse Humidity variations (%)  vs. Latitude
- Demonstrate and analyse Cloudiness variations (%) vs. Latitude
- Demonstrate and analyse  Wind Speed variations (mph) vs. Latitude
- Demonstrate and analyse Temperature variations (F) vs. Latitude-Longitude
- Demonstrate and analyse Humidity variations (%)  vs. Latitude-Longitude
- Demonstrate and analyse Cloudiness variations (%) vs. Latitude-Longitude
- Demonstrate and analyse  Wind Speed variations (mph) vs. Latitude-Longitude

## Data
The evaluation weather data is a collection of current weather data retrieved from 1000 different cities uniformly sampled from across the world.
This data set is collected through [OpenWeatherMap Current Weather API](https://openweathermap.org/current), regularly updated by more than 40,000 weather stations covering over 200,000 cities world wide.

To obtain a uniformly distributed city weather data, cities were sampled by a 2 dimensional uniform latitude-longitude grid sampling scheme.
A uniform linear grid of latitudes and longitudes with fixed spacing was created and a set of uniques cities were uniformly sampled based the vertices of the grid.
The generation of the evaluation data consists of the following stages:

- Create a uniform latitude-longitude grid with fixed equal spacing
- Assign a unique city to each grid vertex
- From collected cities, draw $n$ sample uniformly, at random, without replacement. 

The city to grid assignment was performed by [citipy](https://github.com/wingchen/citipy.git) module.

## Report
The visual report containing the detailed implementation and the discovered insights is available by a Jupyter Noebook [here]().

## Requirements
- python=3.6.5
- jupyter=1.0.0
- notebook=5.4.1
- numpy=1.14.2
- matplotlib=2.2.2
- pandas=0.22.0
- scipy=1.1.0


## Directory Structure
This repo contains three directories: 'fig', 'img' and 'log':

- 'fig': 'png' files of scatter and geo-map plots.
- 'log': 'csv' file containing all weather data retrieved.
- 'img': image files accompany the repo 'README.md' file.

## References
- [OpenWeatherMap Current Weather API](https://openweathermap.org/current)
- [citipy](https://github.com/wingchen/citipy.git)

## License
NA

