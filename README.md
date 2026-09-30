# Weather Monitoring System

A simple Python-based weather monitoring system that collects daily weather data for a selected month and year. The program records rainfall, sunshine duration, wind speed, and humidity for each day, then displays daily summaries, monthly totals, and maximum values.

## Overview

This project allows a user to enter weather information for each day in a chosen month and year. It calculates and prints:

- Daily rainfall values and classification
- Daily sunshine duration and temperature summaries
- Wind speed classification
- Relative humidity classification
- Monthly totals and maxima

The program is designed as an educational console application and uses only Python built-in features.

## Features

- Accepts a year and month from the user
- Calculates the number of days in the selected month
- Prompts for daily weather input for each day
- Tracks the following values:
  - Rainfall in millimeters
  - Temperature in degree Celsius
  - Sunshine in minutes
  - Wind speed in km/h
  - Relative humidity in percentage
- Classifies each day based on weather conditions
- Displays individual day summaries
- Prints monthly totals and maximum values

## Weather Categories Included

### Rainfall
- Extremely heavy rain
- Very heavy rain
- Heavy rain
- Moderate rain
- Light rain
- Very light rain
- No rain

### Temperature / Sunshine
- Extremely hot day
- Moderately hot day
- Less hot day
- Cold day
- Very cold day
- Extremely cold day
- Very sunny day
- Moderately sunny day
- Very less sunny day, partially cloudy
- Very cloudy day

### Wind Speed
- Hurricane
- Violent Storm
- Storm
- Strong Gale
- Gale
- High Wind
- Strong Breeze
- Fresh Breeze
- Moderate Breeze
- Gentle Breeze
- Light Breeze
- Light Air
- Calm

### Humidity
- Fully Saturated
- Sticky/Damp
- Moderate
- Ideal
- Extremely Dry

## Program Workflow

1. The user enters the year.
2. The program determines the number of days in each month, including leap-year handling.
3. The user selects a month.
4. For each day of the month, the program asks for weather data.
5. The program analyzes the input and prints the daily weather status.
6. At the end, it displays the total rainfall, maximum rainfall, maximum temperature, total sunshine, and maximum wind speed/humidity values.

## Example Execution

```python
Enter the required year : 2025
Enter the required month : June
```

The software then prompts the user for data for each day of the month, such as:

```python
Enter temperature of the above date in degree celcius rounded off to one decimal place :
Enter the number of minutes of sunshine for the above date :
Enter the speed of wind on the above date in km/hour :
Enter the relative humidity level on the above date in percentage :
```

## Project Structure

This project is a single Python script containing multiple functions:

- `daily_rainfall()`
- `daily_sunshine()`
- `daily_windspeed()`
- `daily_humidity()`

These functions handle data collection and classification for their respective weather metrics.

## How to Run

1. Make sure Python is installed on your system.
2. Save the code in a file such as `weather_monitoring_system.py`.
3. Run the script from the terminal:

```bash
python weather_monitoring_system.py
```

4. Follow the prompts to enter the required weather details.

## Notes

- The project uses basic console input/output and does not include a graphical user interface (GUI).
- It is suitable for learning Python fundamentals such as:
  - Lists
  - Loops
  - Conditional statements
  - User input handling
  - Data accumulation and comparison
- The code currently supports a simple monthly weather logging workflow and can be extended with features such as:
  - Data saving to files
  - Charts and graphs
  - Monthly summaries in a report format
  - Database storage

## License

This project is provided for educational purposes.

## Conclusion

The Weather Monitoring System is a beginner-friendly Python project that simulates daily weather tracking and reporting. It is useful for understanding how to collect, store, and analyze environmental data in a simple and practical manner.
