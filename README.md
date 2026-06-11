# Supermarket Sales Performance Analysis

Welcome to my first data analysis portfolio project! This repository contains an end-to-end data processing and Exploratory Data Analysis (EDA) framework built to analyze supermarket transaction records from 2019. The project focuses on handling programmatic data cleaning, structured aggregations, and multi-dimensional visual reporting.

## 📁 Repository Architecture

The project directory is explicitly structured to separate raw data components from data transformation and analytical execution environments:

.
├── data/
│   ├── raw_supermarket_sales.csv     # Original, unmodified transactional records
│   └── clean_supermarket_sales.csv   # Sanitized, programmatically normalized dataset
└── ipynb/
    ├── 1_data_cleaning.ipynb          # Pipeline for validation, null handling, and type-casting
    └── 2_exploratory_data_analysis.ipynb # Pipeline for deep statistical visualization & grouping

## 🛠️ Technology Stack & Libraries
* **Language:** Python
* **Data Manipulation:** pandas (Indexing, string parsing, grouping, aggregations)
* **Data Visualization:** matplotlib.pyplot (Canvas controls, custom layouts) & seaborn (Multi-variable hue breakdowns, transactional distributions, error-margin estimations)

---

## 📊 Core Analytical Inquiries & Data Insights

Below is a detailed breakdown of the business metrics analyzed and the structural patterns discovered during the Exploratory Data Analysis:

### 1. Temporal Analysis (Sales by Month)
* **Insight:** Transaction volume and gross revenue peaked sharply at the beginning of the year (Q1), followed by stabilization and flat trends across the remaining months.

### 2. Operational Rhythm (Busiest Day of the Week)
* **Insight:** Tuesday was identified as the highest transactional volume driver across the regular weekly cycle, pinpointing peak store operations.

### 3. Spatial Performance & Geography (Sales by Branch & City)
* **Insight:** Branch C consistently generated the maximum total sales volume compared to Branches A and B. Regionally, the city of Navyitaw achieved the highest overall historical revenue contribution.

### 4. Transactional Modality (Payment Distribution)
* **Insight:** Ewallet options represent the single most utilized payment instrument across customers (34.5%), marginally outpacing traditional Cash payments (34.4%).

### 5. Demographics & Engagement (Dwell Time per Customer Type)
* **Insight:** Registered loyalty program Members maintain significantly longer interaction and dwell times within the supermarket environment compared to regular walk-in ("Normal") shoppers.

### 6. Advanced Inter-Variable breakdowns
* **Product Line Analytics per Gender:** The analysis uncovers detailed product line performance split by gender expression, showing targeted buying behaviors where specific item categories are heavily preferred by one group over another.
* **Monthly Sales per Branch:** Tracks month-over-month performance per branch location, revealing specific structural performance variances distinct to individual storefronts rather than general market trends.

---

## ⚙️ Operational Pipeline Breakdown

### Phase 1: Data Sanitization (1_data_cleaning.ipynb)
* Enforced explicit datetime formatting across raw chronological string attributes (Date, Time).
* Identified, verified, and handled any missing observations or anomalous outliers.
* Validated feature types and stripped inconsistent text formatting from categorical values.
* Exported a production-ready baseline to data/clean_supermarket_sales.csv.

### Phase 2: Exploratory Data Analysis (2_exploratory_data_analysis.ipynb)
* Constructed multi-variate statistical graphics (split-bar configurations, layered trends, and hue matrices).
* Aggregated granular metrics into actionable corporate performance charts.
* Isolated subtle relationships across overlapping transactional dimensions (e.g., cross-analyzing Branch, Time Block, Gender, and revenue).

---

## 📈 Planned Future Updates
To take this introductory project further, future versions of this repository will implement diagnostic analytics:
1. Statistical Validation Tests: Introduce scipy.stats to execute ANOVA tests across store performance ratings and Chi-Square tests to verify whether buying habits are truly dependent on gender.
2. Predictive Machine Learning Modeling: Build a supervised learning model (using scikit-learn) to forecast single basket size thresholds based on real-time transaction timings and location inputs.
