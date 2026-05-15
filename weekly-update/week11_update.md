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

[Back to Home](index.html)
