# Data Science Finals Portfolio - Peter Lee

## About Me
I am a student at Whitman College taking Data Science Class. This is the Final Project for the class.
Through this course, I hope to strengthen my skills in data analysis and visualization, and to build projects that reflect my academic and personal interests.

## Project Idea 1: Weather and Productivity

Questions:
- How does weather (temperature, precipitation, sunlight) affect daily productivity?
- Which weather condition has the strongest relationship with productivity levels?

---

## Project Idea 2: Weather and Physical Activity

Questions:
- How does weather influence physical activity levels?
- Do people exercise less on days with extreme temperatures or rain?

---

## Project Idea 3: Weather and Sleep Patterns

Questions:
- How does temperature affect sleep duration and quality?
- Are extreme weather conditions associated with poorer sleep?

---

## Week 10 Update

I will be working on this project individually.

My general topic is exploring the relationship between **weather conditions and productivity-related behaviors**. Initially, I wanted to directly analyze productivity, but I found that there are no reliable datasets with daily productivity measurements. Therefore, I will instead use **proxy variables for productivity**, such as physical activity or screen time.

### Data Sources

- **Open-Meteo (weather data)**  
  - Pros: Flexible, clean, daily data with location and time control  
  - Cons: Only provides weather variables and must be combined with another dataset  

- **Activity / Screen Time datasets (proxy for productivity)**  
  - Pros: Can represent behavior related to productivity  
  - Cons: May be messy or not perfectly aligned with weather data  

### Research Questions

- How do weather conditions (temperature, precipitation, sunlight) affect activity levels or screen time?  
- Are certain weather conditions associated with more “productive” behaviors?  
- Is there a noticeable trend in behavior changes across different weather patterns?
---

## Week 11 Update

### Data Sources

For my final project, I decided to analyze how weather influences daily productivity-related behavior using two datasets:

1. **Wearable Activity Dataset (Norway, 2019–2020)**  
   - Daily data from 113 participants using Garmin/Fitbit devices  
   - Includes steps, activity levels (light, moderate, vigorous), and sedentary time  

2. **Open-Meteo Weather Data**  
   - Daily weather data (temperature, precipitation, cloud cover, etc.)  
   - Matched to the same date range (2019–2020)  

I chose these datasets because they allow for a real-world, time-aligned comparison between environmental conditions and human behavior.

---

### Data Acquisition

The activity dataset was obtained from a publicly available research dataset.  
The weather data was collected using the Open-Meteo API and exported as a CSV file.

---

### Data Considerations (Strengths & Limitations)

**Strengths:**
- High-resolution daily data  
- Real-world behavioral data from wearable devices  
- Multiple activity variables for richer analysis  

**Limitations:**
- Activity is only a proxy for productivity  
- Missing values (e.g., some devices do not track all variables)  
- Data is averaged across individuals, losing personal variation  
- Dataset is limited to Norway, so results may not generalize  

---

### Preliminary Analysis

I loaded both datasets into Google Colab and inspected their structure.  
Initial exploration showed that:

- Activity data includes multiple participants per day  
- Weather data is already aggregated at the daily level  
- Date formats differ between datasets and need to be standardized  

---

### Data Cleaning & Wrangling

So far, I have identified the following steps:

- Rename columns to improve readability  
- Convert date formats into a consistent datetime format  
- Select relevant variables (steps, activity levels, sedentary time)  
- Aggregate activity data by date (daily population average)  
- Merge activity and weather datasets on date  

I also plan to create a **productivity score** based on activity variables.

---

### Challenges

- Defining a meaningful and defensible productivity metric  
- Handling missing or inconsistent activity data  
- Aligning multiple participants' data with a single daily weather value  
- Ensuring that results are interpretable and not misleading  

---

### Next Steps

- Complete data cleaning and merging  
- Engineer a productivity score  
- Perform correlation and visualization analysis  
- Explore more advanced relationships between weather and activity

---

## Week 12 Update

### Exploratory Analysis

This week, I conducted exploratory analysis on both the activity and weather datasets to better understand their structure and patterns before combining them.

For the activity dataset, I aggregated the data to a daily level by averaging across all participants. I then explored trends in daily steps, distributions of activity levels, and the relationship between sedentary time and steps. The analysis showed a weak negative correlation between sedentary time and steps, suggesting that higher inactivity is associated with lower movement, though the relationship is not strong.

For the weather dataset, I converted hourly data into daily averages and examined temperature trends and precipitation patterns. The data shows clear seasonal variation in temperature and a highly skewed distribution of precipitation, with many days having little to no rainfall.

### Interactive Visualization

I created interactive visualizations using Plotly to explore the data more effectively. These visualizations allow zooming and closer inspection of trends and relationships, making it easier to identify patterns in activity behavior.

### Key Insights

- Daily activity levels show variability over time with some seasonal patterns.
- Sedentary time and steps are negatively related, but only weakly.
- Weather variables, especially temperature, show strong seasonal trends.
- Precipitation is unevenly distributed, with many low values and a few extreme events.

### Next Steps

Next, I will merge the activity and weather datasets by date and analyze how weather conditions influence daily activity behavior.
