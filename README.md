# Social Media Engagement & Performance Analysis

Social Media Engagement &amp; Performance Analysis using Python, Pandas, NumPy, Matplotlib, and Seaborn to analyze user engagement, content performance, audience trends, and social media metrics.


## 📌 Project Overview

The **Social Media Engagement & Performance Analysis** project analyzes social media data to understand audience engagement, content performance, and patterns across different user and content segments.

The project uses data analysis and visualization techniques to study metrics such as **likes, comments, shares, impressions, watch time, follower count, and engagement rate**. It also examines performance based on content type, category, country, age group, sentiment, device type, and posting day.

---

## 🎯 Objective

The main objective of this project is to:

* Analyze overall social media engagement and performance.  
* Identify patterns in likes, comments, shares, impressions, and watch time.  
* Understand factors associated with engagement rate.  
* Compare performance across different content types and categories.  
* Analyze engagement patterns across countries, age groups, sentiments, and devices.  
* Identify unusual values and variations in engagement data.  
* Generate data-driven insights for improving social media performance.  

---

## ❗ Problem Statement

Social media platforms generate large amounts of engagement data, but understanding the factors behind content performance can be challenging.

This project addresses the following problems:

* How is overall social media engagement performing?  
* Which content types generate better engagement?  
* How does performance vary across different content categories?  
* Are there differences in engagement across countries and age groups?  
* How does sentiment relate to audience engagement?   
* Does device type show differences in user engagement behavior?  
* What relationships exist between likes, comments, shares, impressions, watch time, and engagement rate?  
* Are there unusual or extreme engagement values in the dataset?  
* How can the analysis support data-driven social media decisions?  

---

## 📊 Dataset

The dataset contains **5,000 social media records** covering the period from **2022 to 2023**.

### Key Variables

| Variable         | Description                              |
| ---------------- | ---------------------------------------- |
| Age              | Age of the user                          |
| Gender           | Gender of the user                       |
| Content Type     | Type of social media content             |
| Category         | Content category                         |
| Likes            | Number of likes                          |
| Comments         | Number of comments                       |
| Shares           | Number of shares                         |
| Watch Time       | Time spent watching content              |
| Impression Count | Number of impressions                    |
| Follower Count   | Number of followers                      |
| Engagement Rate  | Measure of overall engagement            |
| Sentiment        | Positive, neutral, or negative sentiment |
| Device Type      | Device used by the user                  |
| Country          | User/content country                     |
| Posting Date     | Date of the social media post            |

---

## 🛠️ Technologies Used

* **Python**  
* **Jupyter Notebook**  
* **Pandas** – Data manipulation and analysis  
* **NumPy** – Numerical analysis  
* **Matplotlib** – Data visualization  
* **Seaborn** – Statistical visualization  
* **Plotly** – Interactive visualization

---

## 🔄 Project Workflow

```text
Data Collection
      ↓
Data Loading
      ↓
Data Cleaning
      ↓
Missing Value Treatment
      ↓
Data Transformation
      ↓
Exploratory Data Analysis
      ↓
Statistical Analysis
      ↓
Data Visualization
      ↓
Correlation Analysis
      ↓
Engagement Performance Analysis
      ↓
Insights & Recommendations
```

---

## 🧹 Data Preprocessing

The project includes several data preprocessing steps:

* Checking the structure and data types of the dataset.  
* Identifying missing values.  
* Handling missing values using appropriate imputation techniques.  
* Checking numerical variables for unusual values.  
* Analyzing outliers in engagement-related variables.  
* Applying transformation techniques where required.  
* Creating additional features for analysis.  

---

## 📈 Exploratory Data Analysis

The project analyzes social media performance using different visualizations, including:

* Histogram plots  
* Line plots  
* Pie plots  
* Scatter plots  
* Bar charts      
* Box plots     
* Violin plots  
* Count plot  
* Swarm plots    
* Pair plots     
* Correlation heatmaps    

These visualizations help identify patterns, distributions, differences between groups, and relationships among variables.

---

## 🔍 Correlation Analysis

A correlation heatmap and pair plot are used to study relationships between numerical variables such as:

* Age  
* Likes  
* Comments  
* Shares  
* Watch Time  
* Impression Count  
* Follower Count  
* Engagement Rate  

The analysis shows that most numerical variables have **weak linear relationships with engagement rate**. The strongest observed relationship with engagement rate is between **impression count and engagement rate**, with a correlation of approximately **-0.232**.

This indicates that engagement performance should not be explained using a single numerical metric.

---

## 📊 Key Analysis Areas

### Content Performance

The project compares engagement across:

* Reel  
* Image  
* Text  
* Video  

Video content recorded the highest average engagement rate among the analyzed content types.

### Category Performance

The analysis covers categories such as:

* Fitness  
* Technology  
* Music  
* Education  
* Lifestyle  
* Travel  
* Fashion  
* Food  

### Geographic Analysis

Engagement and impression performance are compared across different countries to identify geographic variations.

### Sentiment Analysis

The project compares:

* Positive  
* Neutral  
* Negative  

sentiment and examines their relationship with engagement metrics.

### Device Analysis

Engagement-related behavior is analyzed across:

* Mobile  
* Tablet  
* Desktop  

### Age Group Analysis

Engagement performance is also compared across different age groups.

---

## 📉 Outlier Analysis

The engagement-rate distribution contains extreme values. The maximum observed engagement rate is approximately **191.50**, while the median is approximately **0.254**.

The analysis identified a large number of potential outliers using the IQR method. Data transformation and winsorization techniques were therefore applied to reduce the influence of extreme observations during analysis.

---

## 🧠 Analytics Approach

The project provides insights at four levels:

### 1. Descriptive Analytics

From a descriptive perspective, average performance was approximately 10,107 likes, 1,502 comments, 1,003 shares, 4,014.5 seconds of watch time, and 0.96 engagement rate. However, the engagement-rate median was only 0.25, revealing strong right skew.

### 2. Diagnostic Analytics

From a diagnostic perspective, the correlation analysis showed that most numerical variables have weak relationships with engagement rate. Impressions had the strongest observed relationship at -0.232, while likes had only 0.094. This indicates that high reach does not necessarily translate into high engagement efficiency. Under 18 age group showing the highest average engagement rate and the 56+ group showing the lowest. Non-verified accounts show slightly higher average engagement rate than verified accounts in this dataset. Mobile has the highest average watch time, while desktop has the lowest. The difference between other devices are relatively small. Negative sentiment posts show higher average engagement in this dataset. Posts published on Tuesday receive the highest average impressions while Thursday has the lowest average impressions. Male users represent the largest share of the dataset.

Content analysis showed that video had the highest average engagement rate (0.49) and highest average likes (10,188.61), while images generated the highest average comments (1,525.39) and shares (1,019.03). At category level, Fitness had the highest engagement rate (0.50), whereas Food had the highest average likes (10,226).

Geographically, India generated the highest average impressions (52,462.39), while Australia recorded the highest average engagement rate (0.53). This further demonstrates the distinction between reach and engagement quality.

### 3. Predictive Analytics

From a predictive perspective, the weak individual correlations suggest that engagement rate should not be predicted using a single variable. A future machine-learning model should combine content type, category, sentiment, demographics, device, posting day, impressions, followers, and other engagement variables.

### 4. Prescriptive Analytics

From a prescriptive perspective, social-media strategy should use multiple KPIs rather than impressions alone. Content should be evaluated separately for reach, likes, comments, shares, watch time, and engagement rate. Fitness and video content warrant further investigation based on their observed engagement performance, while Tuesday may be tested for visibility because it produced the highest average impressions.

---

## 💡 Key Insights

* Social media engagement varies across different content types and categories.
* Video content showed the highest average engagement rate among the content types analyzed.
* Fitness showed the highest average engagement rate among the analyzed categories.
* Engagement rate has a highly skewed distribution with extreme observations.
* Most numerical variables have weak linear relationships with engagement rate.
* Impression count showed the strongest observed relationship with engagement rate.
* Device type provides useful segmentation information but does not by itself explain engagement performance.
* Multiple factors should be considered together when evaluating social media performance.

---

## ✅ Conclusion

The **Social Media Engagement & Performance Analysis** provides a comprehensive view of social media performance using engagement, audience, content, geographic, sentiment, and device-related variables.

The analysis demonstrates that social media engagement cannot be explained by a single metric. Combining multiple dimensions provides a better understanding of content performance and audience behavior.

The insights generated from this project can support **data-driven content planning, performance monitoring, audience analysis, and future social media strategy development**.

---

## 📁 Project Structure

```text
Social-Media-Engagement-&-Performance-Analytics/
│
├── Social_Media_Engagement_& performance_Analytics.ipynb
├── README.md
└── dataset/
    └── social_media_data.csv
```

---

## 👩‍💻 Author

**Shanthini**

Social Media Engagement & Performance Analysis Project

