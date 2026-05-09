# Week 12 Update

[Back to Home](index.html)

## Exploratory Analysis and Updated Research Question

This week, I revised my analysis based on feedback. Instead of averaging all participants together, I divided the 113 participants into low-, medium-, and high-activity groups based on their average daily steps.

My updated research question is:

**Do weather conditions affect low-, medium-, and high-activity participants differently?**

## Weather Data Exploration

Before merging the datasets, I explored the weather data separately.

The weather dataset covers 731 days from 2019 to 2020 and has no missing values. I focused on three weather variables:

- Temperature
- Precipitation
- Cloud cover

The temperature data showed a clear seasonal pattern, with colder winter months and warmer summer months. Precipitation was strongly right-skewed, meaning most days had little precipitation while a few days had higher values. Cloud cover was generally high, with about 52.8% of days classified as cloudy using a 75% threshold.

## Activity Grouping

Participants were divided into three groups based on their average daily steps:

- Low-activity group: about 6,349 steps per day
- Medium-activity group: about 9,406 steps per day
- High-activity group: about 13,015 steps per day

This grouping created clear differences between participants and made the analysis more meaningful.

## Merging Activity and Weather Data

I aggregated the activity data by date and activity group, then merged it with the daily weather data by date.

The final merged dataset has 2,193 rows:

- 731 days
- 3 activity groups per day
- No missing values after merging

This means the merged data is clean and ready for analysis.

## Main Finding: Temperature and Activity

The clearest pattern was between temperature and average daily steps. Across all three activity groups, average steps generally increased as temperature became warmer.

This suggests that warmer weather is associated with higher physical activity. However, the three groups remained clearly separated, meaning that baseline activity level still matters.

## Other Weather Variables

Precipitation did not show a strong relationship with steps. Average steps were very similar on days with and without measurable precipitation.

Cloud cover showed a mild pattern. Very cloudy days were associated with slightly lower steps, especially for medium- and high-activity participants, but the pattern was not as strong as temperature.

## Interactive Visualization

The interactive visualization below shows the relationship between daily temperature and average daily steps by activity group.

<iframe 
  src="temperature_steps_scatter_plotly.html" 
  width="100%" 
  height="700" 
  frameborder="0">
</iframe>

## Key Insights

- Temperature had the clearest relationship with daily steps.
- Average steps increased on warmer days across all activity groups.
- Precipitation did not appear to strongly affect steps.
- Very cloudy days were associated with slightly lower activity.
- Low-, medium-, and high-activity participants stayed clearly separated, even when weather changed.

## Next Steps

Next, I would like to refine the analysis by controlling for seasonality and exploring whether weather affects not only steps, but also sedentary time and moderate or vigorous activity minutes.
