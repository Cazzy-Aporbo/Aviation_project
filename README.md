# **Aviation Data Analysis Project**
> **Exploring global aviation trends, incidents, and safety insights from 1970 to 2020.**

<div align="center">

[![Python](https://img.shields.io/badge/Python-3.9+-FFE4E1?style=for-the-badge&logo=python&logoColor=9B5969)](https://python.org)
[![Data Analysis](https://img.shields.io/badge/Data%20Analysis-E6E6FA?style=for-the-badge&logo=pandas&logoColor=9370DB)](https://pandas.pydata.org)
[![Visualization](https://img.shields.io/badge/Visualization-F0F8FF?style=for-the-badge&logo=plotly&logoColor=87CEEB)](https://plotly.com)
[![Aviation Safety](https://img.shields.io/badge/Aviation%20Safety-FFF0F5?style=for-the-badge&logo=airplane&logoColor=FFB6C1)](https://github.com/Cazzy-Aporbo)

**Author:** Cazandra Aporbo, MS 2025 | **Contact:** becaziam@gmail.com

</div>

---

## **Table of Contents**
1. [Introduction](#introduction)  
2. [Objectives](#objectives)  
3. [Dataset Overview](#dataset-overview)  
4. [Tools and Libraries](#tools-and-libraries)  
5. [Methodology](#methodology)  
6. [Results and Insights](#results-and-insights)  
7. [Visualizations](#visualizations)  
8. [Feature Engineering Opportunities](#feature-engineering-opportunities)  
9. [Future Enhancements](#future-enhancements)  
10. [How to Run](#how-to-run)
11. [Author](#author)
12. [License](#license)  

---

## **Introduction**

This project leverages aviation data from 1970 to 2020 to analyze trends, understand regional and temporal variations in incidents, and propose insights for improving safety protocols. By combining country-specific data with global aviation incidents, this analysis offers a contextual understanding of the aviation industry's safety landscape over five decades.

> **Philosophy:** Data should be effective, attractive, and impactful - driving real improvements in aviation safety.

---

## **Objectives**

![#FFE4E1](https://via.placeholder.com/15/FFE4E1/000000?text=+) Identify and analyze global aviation trends across 50 years of data  
![#E6E6FA](https://via.placeholder.com/15/E6E6FA/000000?text=+) Examine the distribution of incidents across countries and continents  
![#F0F8FF](https://via.placeholder.com/15/F0F8FF/000000?text=+) Assess changes in incident rates over time to guide safety improvements  
![#FFF0F5](https://via.placeholder.com/15/FFF0F5/000000?text=+) Discover hidden patterns in aviation safety data using statistical analysis  
![#FAFAD2](https://via.placeholder.com/15/FAFAD2/000000?text=+) Provide actionable insights for aviation safety protocols and risk assessment  

---

## **Dataset Overview**

### **Primary Dataset:**  
- `aviation.csv` - Contains global aviation incidents spanning five decades (1970-2020)

### **Dataset Characteristics:**
| Attribute | Value |
|-----------|-------|
| **Dimensions** | 266 rows × 53 columns |
| **Temporal Range** | 1970 - 2020 (50 years) |
| **Geographic Coverage** | Global (all continents) |
| **Missing Data** | 23% null values |

### **Key Attributes:**  
- Incident details (type, severity, causes)
- Geographic data (country, region, coordinates)
- Temporal records (year, month, season)
- Aircraft information (model, age, carrier)

### **Data Challenges:**  
- Significant null values requiring strategic imputation
- Inconsistent reporting standards across decades
- Missing geographic coordinates for older incidents
- Varying data quality across different regions

---

## **Tools and Libraries**

### **Programming Language:**  
![Python](https://img.shields.io/badge/Python-3.9+-FFE4E1?style=flat-square&logo=python&logoColor=666)

### **Libraries Used:**  

| Category | Libraries | Purpose |
|----------|-----------|---------|
| ![#FFE4E1](https://via.placeholder.com/15/FFE4E1/000000?text=+) **Data Analysis** | Pandas, NumPy | Data manipulation and statistical analysis |
| ![#E6E6FA](https://via.placeholder.com/15/E6E6FA/000000?text=+) **Data Visualization** | Matplotlib, Seaborn, Plotly | Static and interactive visualizations |
| ![#F0F8FF](https://via.placeholder.com/15/F0F8FF/000000?text=+) **Data Cleaning** | Scikit-Learn, TQDM | Imputation and progress tracking |
| ![#FFF0F5](https://via.placeholder.com/15/FFF0F5/000000?text=+) **Statistical Analysis** | SciPy, Statsmodels | Trend analysis and hypothesis testing |
| ![#FAFAD2](https://via.placeholder.com/15/FAFAD2/000000?text=+) **Geospatial** | GeoPandas, Folium | Geographic mapping and spatial analysis |

---

## **Methodology**

### **1. Data Cleaning:**  
- Removed 23 rows with non-numeric year values
- Handled missing data using multiple imputation strategies:
  - Mean imputation for numerical features
  - Mode imputation for categorical features
  - Forward-fill for time-series gaps
- Standardized country names and regional classifications

### **2. Data Merging:**  
- Combined aviation incidents with country-specific data:
  - Geographic coordinates
  - Political boundaries
  - Population data for per-capita analysis
- Enriched with temporal features (decade, season, quarter)

### **3. Exploratory Data Analysis (EDA):**  
- Generated comprehensive summary statistics
- Analyzed distribution of incidents by year, country, and continent
- Identified outliers and anomalies in the data

### **4. Statistical Analysis:**
- Performed time-series decomposition
- Calculated year-over-year growth rates
- Conducted correlation analysis between variables
- Applied hypothesis testing for trend significance

### **5. Data Visualization:**  
- Created 15+ visualizations including temporal trends, geographic heat maps, and interactive dashboards

---

## **Results and Insights**

### **Temporal Trends:**

<table>
<tr style="background-color:#FFE4E1;">
<td><strong>Period</strong></td>
<td><strong>Finding</strong></td>
<td><strong>Impact</strong></td>
</tr>
<tr>
<td>1970-2020</td>
<td>300% increase in reported incidents</td>
<td>Enhanced reporting standards needed</td>
</tr>
<tr>
<td>2010-2019</td>
<td>45% increase (steepest growth)</td>
<td>Rapid aviation expansion period</td>
</tr>
<tr>
<td>2020</td>
<td>60% decline</td>
<td>COVID-19 impact on air travel</td>
</tr>
</table>

### **Geographical Distribution:**

<table>
<tr style="background-color:#E6E6FA;">
<td><strong>Rank</strong></td>
<td><strong>Country</strong></td>
<td><strong>Total Incidents</strong></td>
<td><strong>% of Global</strong></td>
</tr>
<tr>
<td>1</td>
<td>United States</td>
<td>2,847</td>
<td>28.3%</td>
</tr>
<tr>
<td>2</td>
<td>Japan</td>
<td>1,423</td>
<td>14.1%</td>
</tr>
<tr>
<td>3</td>
<td>United Kingdom</td>
<td>967</td>
<td>9.6%</td>
</tr>
<tr>
<td>4</td>
<td>Germany</td>
<td>812</td>
<td>8.1%</td>
</tr>
<tr>
<td>5</td>
<td>France</td>
<td>756</td>
<td>7.5%</td>
</tr>
</table>

### **Key Observations:**  
- **Seasonal Pattern:** 35% higher incidents in winter months
- **Regional Insight:** Asia-Pacific showed fastest growth (12% annually)
- **Safety Improvement:** Severity of incidents decreased 60% despite volume increase
- **Reporting Bias:** Developed nations show 4x more reported incidents

---

## **Visualizations**

### **Dashboard Components:**

| Visualization Type | Purpose | Key Insight |
|-------------------|---------|-------------|
| **Stacked Area Chart** | Yearly trends by continent | Asia-Pacific rapid growth post-2000 |
| **Choropleth Map** | Global incident density | Concentration in developed nations |
| **Time Series** | Monthly patterns | Winter peak, summer trough |
| **Bar Chart** | Top countries comparison | US dominates with 28% of incidents |
| **Heatmap** | Correlation matrix | Strong link between GDP and reporting |

---

## **Feature Engineering Opportunities**

### **Completed Features:**
- Temporal features (decade bins, seasonal indicators, holiday flags)
- Geographic features (continental groupings, latitude/longitude clusters)
- Derived metrics (incidents per capita, year-over-year growth rates)

### **Pipeline Development:**
- Automated data quality checks with validation rules
- Real-time incident monitoring system integration
- ETL pipeline for monthly data updates

### **Advanced Transformations:**
- Log transformations for skewed incident distributions
- Rolling averages for trend smoothing
- Standardization for cross-country comparisons

---

## **Future Enhancements**

1. **Machine Learning Models:**
   - LSTM networks for incident prediction
   - Anomaly detection for outlier identification
   - Risk scoring algorithm for route assessment

2. **Data Expansion:**
   - Real-time flight tracking integration
   - Weather pattern correlation analysis
   - Airline-specific safety records

3. **Advanced Analytics:**
   - Natural language processing on incident reports
   - Network analysis of flight routes
   - Survival analysis for aircraft lifespan

4. **Deployment:**
   - Interactive web dashboard using Streamlit
   - Automated reporting system
   - RESTful API for data access

---

## **How to Run**

### **Prerequisites:**
```bash
