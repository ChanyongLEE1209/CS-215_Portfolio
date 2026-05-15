# Week 14 Update

## Project Progress So Far

My final project explores how weather conditions affect daily productivity-related behavior. Since productivity is difficult to measure directly, I am using physical activity as a proxy for daily behavior.

So far, I have cleaned and combined two datasets:

1. **Norway wearable activity dataset, 2019–2020**
   - 113 participants
   - Daily steps, light activity, moderate activity, vigorous activity, and sedentary time

2. **Open-Meteo weather dataset**
   - Daily weather data matched to the same 2019–2020 date range
   - Temperature, precipitation, and cloud cover

Based on feedback, I changed my approach. Instead of averaging all 113 participants into one daily value, I divided participants into three groups based on their average daily steps:

- Low-activity group
- Medium-activity group
- High-activity group

This helped make my research question more specific:

**Do weather conditions affect low-, medium-, and high-activity participants differently?**

So far, I have completed:

- Cleaning and renaming activity columns
- Converting date formats
- Aggregating hourly weather data into daily weather data
- Exploring temperature, precipitation, and cloud cover
- Creating low-, medium-, and high-activity groups
- Merging grouped activity data with weather data
- Creating static graphs in Matplotlib
- Creating interactive Plotly visualizations for my project website

The main pattern I found so far is that average daily steps tend to increase as temperature becomes warmer. This pattern appears across all three activity groups, although the groups remain clearly separated. Precipitation does not show a strong relationship with steps, while very cloudy days may be associated with slightly lower activity.

## What Remains To Be Done

The main work remaining is to strengthen the analysis and organize the final story clearly.

I still need to:

- Add a statistical model to support the visual patterns
- Interpret the model results carefully
- Improve the final project webpage design and organization
- Decide which visualizations are most important for the final presentation
- Write a clear final conclusion
- Prepare the final class presentation

## New Technique: Multiple Linear Regression with Interaction Terms

<iframe 
  src="regression_temperature_activity_group.html" 
  style="width:100%; height:680px; border:none;">
</iframe>

For my new technique, I plan to use **multiple linear regression with interaction terms**.

So far, most of my analysis has been visual. The graphs suggest that warmer days are associated with more steps, but I want to test this pattern more carefully. I also want to know whether the relationship between temperature and steps is different for low-, medium-, and high-activity participants.

The model I plan to use is:

```text
steps ~ temperature * activity_group + precipitation + cloud_cover

## Communication Strategy

For my final project, I plan to organize the narrative as a clear data story. I will begin by explaining the problem: productivity is difficult to measure directly, so I use physical activity as a proxy for productivity-related behavior. Then I will introduce the two datasets, explain how I cleaned and merged them, and show why I divided participants into low-, medium-, and high-activity groups.

The visuals will be sequenced from broad exploration to final analysis. I will first show weather exploration graphs, such as monthly temperature trends, precipitation distribution, and cloud cover distribution. Then I will show the activity group comparison to explain the low-, medium-, and high-activity categories. After that, I will present the main results: temperature versus steps by activity group, followed by the interactive Plotly scatter plot and the regression prediction graph.

For the class presentation, I plan to present directly from my project web page rather than making a separate slide deck. This will allow me to show the narrative, static graphs, and interactive Plotly visualizations in one place. I may prepare a short outline for myself so that the presentation stays organized, but the website will be the main presentation tool.

[Back to Home](index.html)
