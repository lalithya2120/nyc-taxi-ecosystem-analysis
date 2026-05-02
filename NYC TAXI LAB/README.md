# NYC Taxi Ecosystem Analysis

This project investigates the NYC Yellow Taxi ecosystem using official NYC Taxi and Limousine Commission trip record data.

## Dataset

Source: NYC Taxi and Limousine Commission Trip Record Data  
Taxi type: Yellow Taxi Trip Records  
Months analyzed: April, May, and June 2025

The original raw Parquet files are not included in this repository because they are large. The analysis uses summary CSV files generated from the raw TLC data.

## Project Structure

- `taxi_analysis.ipynb`: Jupyter Notebook containing data cleaning, hypothesis testing, time-based analysis, and simulation
- `NYC_Taxi_Report.pbix`: Power BI decision report
- `data_quality_summary.csv`: Summary of retained and removed records
- `daily_summary.csv`: Daily trip volume and average metrics
- `hourly_summary.csv`: Hourly trip volume and average metrics
- `weekday_summary.csv`: Weekday trip volume and average metrics
- `act5_simulation_summary.csv`: Fare increase simulation results

## Analysis Overview

The project is organized into six acts:

1. Act 1: Roll-number based month selection
2. Act 2: Raw data inspection and cleaning
3. Act 3: Passenger tipping behavior hypothesis test
4. Act 4: Time-based system rhythm analysis
5. Act 5: 5% fare increase simulation
6. Act 6: Power BI decision report

## Key Findings

- The selected month range was April to June based on the roll number calculation.
- The raw dataset required cleaning to define what counts as a real trip.
- Long trips received higher tip amounts, but short trips had higher tip percentages.
- Taxi demand followed a clear daily and weekly rhythm.
- A simulated 5% fare increase raised fare revenue under the assumption that trip volume remains constant.
- Careless interpretation can lead to misleading conclusions, especially around tipping behavior and policy simulation.
