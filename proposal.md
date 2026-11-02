**Team:** Maddie and Dustin

## Research question
How many days reached 90°F or higher in Boulder, Colorado, each summer (June to August) from 1980 to 2025, and has that number increased over time? We expect more 90°F+ days in the 2010s and 2020s than in the 1980s, with the hottest summers clustered in recent years.

## Data
Daily maximum temperatures for Boulder from the Open-Meteo Historical Weather API (https://open-meteo.com/en/docs/historical-weather-api). One record per day from June 1 to August 31, 1980 to 2025 (4,232 records), collected with 46 requests (one per summer) using Python's requests library and pandas. Data is CC BY 4.0, credited as "Weather data by Open-Meteo.com."

## Plan
- Collect the daily temperature data through the API, pausing 1 second between requests, and save it to CSV (Dustin)
- Count 90°F+ days per summer, compare decades, and calculate the trend with a linear regression (both)
- Build a bar chart of 90°F+ days per year, a decade comparison, and a line chart of the average summer high (Maddie)

## Biggest risk
Open-Meteo data is modeled from a grid, not measured at a station, so it may undercount hot days. Our fallback is to compare against NOAA station data for Boulder.
