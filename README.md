# CS215 Portfolio - Peter Lee

## About Me
I am a student at Whitman College majoring in Physics with an interest in engineering and data science. I enjoy exploring how data can be used to understand real-world problems, especially in areas like technology, education, and human behavior. 

Through this course, I hope to strengthen my skills in data analysis and visualization, and to build projects that reflect my academic and personal interests.

## Final Project Ideas

### 1. Topic: Social Media & User Behavior
Dataset: TikTok / Instagram usage datasets (e.g., Kaggle social media usage data)

- How does daily screen time correlate with reported happiness levels?
- Does the type of content (entertainment vs educational) affect engagement time?

---

### 2. Topic: Student Performance & Lifestyle
Dataset: Student performance dataset (e.g., Kaggle student alcohol consumption dataset)

- How does sleep duration affect GPA or test scores?
- Is there a relationship between alcohol consumption and academic performance?

---

### 3. Topic: Health & Physical Activity
Dataset: Fitness tracking dataset (e.g., Fitbit or WHO activity datasets)

- Does exercise frequency correlate with resting heart rate?
- How does physical activity level relate to reported stress levels?

---

## Week 10 Update

### Project Plan

For my final project, I will be working **individually**.

My general topic is **Student Performance and Lifestyle**, focusing on how different daily habits influence academic outcomes.

---

### Dataset

I will be using the **Student Alcohol Consumption dataset from Kaggle**.

This dataset includes variables such as:
- Study time
- Alcohol consumption (weekday and weekend)
- Social activities (going out)
- Absences
- Final grades

---

### Pros and Cons of Dataset

**Pros:**
- Contains multiple relevant variables related to student lifestyle and performance
- Clean and well-structured dataset
- Suitable for correlation and regression analysis

**Cons:**
- Based on self-reported data (possible bias)
- Limited demographic (students in Portugal)
- May not fully represent all student populations

---

### Research Questions

1. How does alcohol consumption affect students’ academic performance (final grades)?
2. Is there a relationship between study time and academic performance?
3. Do social behaviors (such as going out) negatively impact academic outcomes?

---

### Project Goal

Through this project, I aim to analyze how lifestyle factors such as study habits, alcohol consumption, and social behavior influence academic performance using data analysis and visualization techniques. I may also apply basic regression models to better understand these relationships.

---
## Week 11 Update

### Data Source

For this project, I decided to use the **Student Alcohol Consumption dataset from Kaggle**. I chose this dataset because it includes multiple variables related to students’ lifestyle behaviors (such as study time, alcohol consumption, and social activity) along with academic performance (final grades). This makes it well-suited for exploring relationships between daily habits and student outcomes.

---

### Data Acquisition

I obtained the dataset from Kaggle and uploaded it into a Google Colab notebook. I then used Python (pandas) to load and inspect the data. The dataset contains 395 student records and 33 variables.

---

### Data Provenance and Considerations

The dataset was collected through surveys of secondary school students in Portugal and was originally compiled by P. Cortez and A. Silva (2008). Because the data is self-reported, it may contain bias or inaccuracies in how students report behaviors such as alcohol consumption or study time.

Additionally, since the dataset is limited to students in Portugal, the results may not be generalizable to other populations or educational systems.

---

### Exploratory Analysis

From my initial analysis, I examined summary statistics and correlations between key variables. I found that most lifestyle variables have very weak relationships with academic performance.

Study time shows a slight positive relationship with final grades, while social activity (going out) has a small negative relationship. Alcohol consumption (both weekday and weekend) shows little to no meaningful correlation with academic performance.

Overall, the data suggests that these lifestyle factors alone do not strongly explain variation in student grades.

---

### Data Cleaning / Wrangling

The dataset does not contain missing values, so no major cleaning was required at this stage. However, several preprocessing steps are still necessary.

Many variables are ordinal (scaled values from 1–5), meaning they represent categories rather than precise quantities. These must be interpreted carefully in analysis. Additionally, categorical variables (such as gender or job type) may need to be converted into numerical form if used in modeling.

I also plan to create new variables, such as a combined alcohol consumption measure (e.g., total alcohol = Dalc + Walc), to better represent overall behavior.

---

### Limitations

This dataset has several limitations. First, it is based on self-reported survey data, which may introduce bias. Second, the dataset only includes students from a specific region (Portugal), limiting generalizability.

Additionally, many variables are ordinal, which restricts the types of statistical analysis that can be applied. Finally, correlation analysis does not imply causation, so observed relationships cannot be interpreted as cause-and-effect.

---

### Challenges

One challenge is that the dataset does not show strong relationships between variables, making it difficult to draw clear conclusions. Another challenge is that many variables are ordinal rather than continuous, which limits analytical approaches.

Moving forward, a key challenge will be identifying meaningful patterns and potentially applying more advanced methods to better understand the data.
