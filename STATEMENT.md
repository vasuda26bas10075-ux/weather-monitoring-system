# Weather Monitoring System - Problem Statement

## Project Title
Weather Monitoring System

## Objective
To develop a Python-based application that collects and analyzes daily weather data for a given month and year. The system monitors and classifies various meteorological parameters including rainfall, temperature, sunshine duration, wind speed, and humidity levels.

## Problem Description
Weather monitoring is essential for understanding climate patterns, predicting weather conditions, and planning agricultural and outdoor activities. This project aims to create a simple yet effective system that allows users to:

1. Input daily weather measurements for a complete month
2. Track and store weather data systematically
3. Classify weather conditions based on established meteorological standards
4. Generate monthly summaries and reports
5. Identify extreme weather events and maximum values

## Scope of the System

### Data Collection
The system collects the following daily weather parameters:

1. **Rainfall**: Amount in millimeters (rounded to one decimal place)
2. **Temperature**: In degree Celsius (rounded to one decimal place)
3. **Sunshine Duration**: In minutes
4. **Wind Speed**: In km/hour
5. **Relative Humidity**: In percentage

### Data Analysis
The system performs the following analyses:

1. **Rainfall Analysis**
   - Classifies daily rainfall into 7 categories
   - Calculates total monthly rainfall
   - Identifies maximum rainfall in a single day

2. **Temperature and Sunshine Analysis**
   - Classifies daily temperature into 6 categories
   - Classifies daily sunshine duration into 4 categories
   - Calculates total monthly sunshine
   - Identifies maximum temperature and sunshine values

3. **Wind Speed Analysis**
   - Classifies wind speed into 13 categories based on the Beaufort scale
   - Identifies maximum wind speed in the month

4. **Humidity Analysis**
   - Classifies humidity levels into 5 categories
   - Identifies maximum humidity level in the month

## Functional Requirements

### Input Requirements
1. User must provide the year (as an integer)
2. User must provide the month (as a string, e.g., "January", "February")
3. For each day of the selected month, the user must provide:
   - Rainfall amount
   - Temperature
   - Sunshine duration
   - Wind speed
   - Relative humidity

### Processing Requirements
1. **Leap Year Handling**: The system must correctly calculate February as having 29 days in leap years
2. **Data Validation**: The system must validate that the entered month exists in the month dictionary
3. **Data Storage**: All daily values must be stored in lists for calculation and display purposes
4. **Classification**: Weather conditions must be classified according to predefined thresholds
5. **Calculation**: The system must calculate:
   - Total rainfall for the month
   - Maximum rainfall in a single day
   - Maximum temperature
   - Total sunshine minutes
   - Maximum sunshine in a single day
   - Maximum wind speed
   - Maximum humidity level

### Output Requirements
1. Display each date in DD/MM/YYYY format
2. Show daily weather classification for each parameter
3. Display all daily measurements in list format
4. Show monthly totals and maximum values
5. Present results in an easy-to-read format

## Weather Classification Thresholds

### Rainfall Classification (in mm)
- **Extremely Heavy Rain**: > 150.0 mm
- **Very Heavy Rain**: 70.0 - 150.0 mm
- **Heavy Rain**: 30.0 - 70.0 mm
- **Moderate Rain**: 10.0 - 30.0 mm
- **Light Rain**: 1.0 - 10.0 mm
- **Very Light Rain**: 0.0 - 1.0 mm
- **No Rain**: 0.0 mm

### Temperature Classification (in °C)
- **Extremely Hot Day**: ≥ 35.0 °C
- **Moderately Hot Day**: 25.0 - 35.0 °C
- **Less Hot Day**: 16.0 - 25.0 °C
- **Cold Day**: 5.0 - 16.0 °C
- **Very Cold Day**: 0.0 - 5.0 °C
- **Extremely Cold Day**: < 0.0 °C

### Sunshine Duration Classification (in minutes)
- **Very Sunny Day**: ≥ 480 minutes
- **Moderately Sunny Day**: 240 - 480 minutes
- **Very Less Sunny Day, Partially Cloudy**: 0 - 240 minutes
- **Very Cloudy Day**: 0 minutes

### Wind Speed Classification (Beaufort Scale, in km/h)
- **Hurricane**: ≥ 118 km/h
- **Violent Storm**: 103 - 118 km/h
- **Storm**: 89 - 103 km/h
- **Strong Gale**: 75 - 89 km/h
- **Gale**: 62 - 75 km/h
- **High Wind**: 50 - 62 km/h
- **Strong Breeze**: 40 - 50 km/h
- **Fresh Breeze**: 30 - 40 km/h
- **Moderate Breeze**: 20 - 30 km/h
- **Gentle Breeze**: 12 - 20 km/h
- **Light Breeze**: 6 - 12 km/h
- **Light Air**: 1 - 6 km/h
- **Calm**: 0 km/h

### Humidity Classification (in %)
- **Fully Saturated**: 70 - 100%
- **Sticky/Damp**: 60 - 70%
- **Moderate**: 50 - 60%
- **Ideal**: 30 - 50%
- **Extremely Dry**: < 30%

## System Functions

### 1. daily_rainfall()
Collects rainfall data for each day of the month, calculates totals and maxima, and displays daily rainfall classifications.

### 2. daily_sunshine()
Collects temperature and sunshine data for each day, calculates totals and maxima, and displays daily temperature and sunshine classifications.

### 3. daily_windspeed()
Collects wind speed data for each day, classifies it according to the Beaufort scale, and identifies maximum wind speed.

### 4. daily_humidity()
Collects relative humidity data for each day, classifies it into humidity levels, and identifies maximum humidity.

## Program Execution Flow
1. User enters the required year
2. System validates and accepts the month input
3. System determines the number of days in the selected month
4. For each day, the user is prompted to enter weather data
5. System processes data and displays daily classifications
6. System displays monthly summaries and extreme values

## Technical Specifications
- **Language**: Python
- **User Interface**: Console-based (command-line)
- **Data Structure**: Lists for storing daily measurements
- **Input Method**: Standard input (keyboard)
- **Output Method**: Console output (print statements)

## Limitations
1. No graphical user interface (GUI)
2. No data persistence (data is not saved to files)
3. No database integration
4. Manual data entry for each day
5. No error handling for invalid numeric inputs
6. Single-month processing per execution
7. Limited input validation

## Future Enhancements
1. **Data Persistence**: Save weather data to CSV or database files
2. **Data Visualization**: Generate charts and graphs for weather trends
3. **Historical Comparison**: Compare current month with previous months/years
4. **Predictive Analysis**: Use data to predict future weather patterns
5. **Error Handling**: Implement robust error handling and input validation
6. **GUI Development**: Create a graphical user interface for better usability
7. **API Integration**: Fetch real weather data from online weather services
8. **Report Generation**: Generate monthly weather reports in PDF format
9. **Multi-month Analysis**: Support analysis across multiple months
10. **Data Export**: Export weather data in various formats (CSV, JSON, Excel)

## Learning Outcomes
This project helps students learn:
- Python fundamentals (variables, data types, loops, conditionals)
- List data structures and manipulation
- Function definition and calling
- User input/output handling
- Conditional logic and comparison operators
- Data accumulation and statistical calculations
- Code organization and modular programming
- Problem-solving and logical thinking

## Conclusion
The Weather Monitoring System is a practical educational project that simulates real-world weather data collection and analysis. It demonstrates fundamental programming concepts while solving a meaningful problem related to environmental monitoring and weather tracking.
