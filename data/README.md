# Data

`sample_cleaned.csv` is a 20-row random sample of the cleaned dataset. The full dataset (4,232 rows) is created by running `analysis.ipynb`.

Weather data by Open-Meteo.com (CC BY 4.0).

## Data dictionary

| Field | Type | Description |
|---|---|---|
| `date` | date (YYYY-MM-DD) | The calendar day, in Boulder local time (America/Denver) |
| `year` | integer | The summer the day belongs to (1980 to 2025) |
| `month` | integer | Month of the day: 6 = June, 7 = July, 8 = August |
| `temp_max_f` | decimal | That day's highest air temperature 2 meters above ground, in °F, rounded to 1 decimal (Open-Meteo `temperature_2m_max`) |
| `hot_day` | True/False | True if `temp_max_f` is 90°F or higher |
