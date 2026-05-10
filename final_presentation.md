# Weather and Daily Activity

## Introduction
Weather affects our daily routines, but productivity is difficult to measure directly. In this project, I use physical activity as a proxy for productivity-related behavior.

## Research Question
Do weather conditions affect low-, medium-, and high-activity participants differently?

## Data
I used two datasets:
1. Norway wearable activity dataset from 2019–2020
2. Open-Meteo weather data from the same date range

## Data Cleaning and Wrangling
The activity data was daily participant-level data, while the weather data was hourly. I aggregated the weather data into daily averages, cleaned the date columns, grouped participants by average step count, and merged the datasets by date.

## Main Visualizations
[Put your key graphs here]

## New Technique
For my new technique, I used multiple linear regression with interaction terms. This allowed me to examine whether the relationship between temperature and steps changed depending on activity group.

## Main Findings
1. Warmer days were generally associated with higher average daily steps.
2. High-activity participants remained more active across weather conditions.
3. Precipitation had a weaker effect than expected.
4. Cloud cover showed a slight negative relationship with daily activity.

## Limitations
This project shows association, not causation. Physical activity is only a proxy for productivity, not a direct measure of productivity.

## Reflection
The hardest part was merging two datasets with different time structures. If I had more time, I would add direct productivity measures like study time, sleep, or screen time.
