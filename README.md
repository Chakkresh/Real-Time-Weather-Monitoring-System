# Real-Time Weather Retrieval System

## Overview

The Real-Time Weather Retrieval System is a ServiceNow scoped application that retrieves current weather information for a city through Open-Meteo REST APIs and stores the results in a custom Weather Data table.

This project demonstrates ServiceNow application development, REST API integration, server-side scripting, JSON parsing, validation, and reporting.

## Features

- Search for weather information by city name.
- Retrieve city latitude, longitude, and region.
- Fetch current temperature in Celsius.
- Integrate external APIs using ServiceNow REST Messages.
- Process API responses using a Script Include.
- Trigger weather retrieval through a UI Action.
- Validate user input and handle API errors.
- Store successful results in the Weather Data table.
- View stored information through reports and dashboards.

## Technologies Used

- ServiceNow Studio
- JavaScript
- ServiceNow REST Messages
- Script Includes and UI Actions
- JSON
- Open-Meteo APIs
- ServiceNow Reports and Dashboards

## API Integration

### Geocoding API

Retrieves the city's coordinates and administrative region.

### Current Weather API

Retrieves current weather information using latitude and longitude.

## How It Works

1. The user opens the Weather Data form in ServiceNow.
2. The user enters a city name.
3. The user clicks the Find Weather UI Action.
4. The WeatherService Script Include calls the Geocoding API.
5. ServiceNow extracts the city's latitude, longitude, and region.
6. ServiceNow calls the Current Weather API.
7. The returned JSON is parsed to obtain the temperature.
8. The UI Action populates the Weather Data fields.
9. The record is saved after successful weather retrieval.
10. Stored information can be reviewed through configured reports and dashboards.

## Main Components

- **Weather Geocoding API:** Retrieves city details and coordinates.
- **Weather Current API:** Retrieves current temperature.
- **WeatherService Script Include:** Handles API requests, JSON parsing, and error responses.
- **Find Weather UI Action:** Initiates retrieval, populates fields, and saves successful results.
- **Client Script:** Validates that the location field is provided.
- **Reports and Dashboard:** Help review stored weather information.

## Learning Outcomes

This project provides practical experience with ServiceNow scoped applications, REST API integration, JavaScript, JSON parsing, form validation, server-side scripting, error handling, and reporting.

## Future Enhancements

- Add humidity and wind speed.
- Store historical weather readings.
- Schedule periodic weather retrieval.
- Add more weather visualizations.
- Improve automated testing and monitoring.

## Author

**Chakkresh S K**

ServiceNow Developer
