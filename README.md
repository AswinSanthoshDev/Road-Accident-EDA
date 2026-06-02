# Kerala Road Accident Analysis EDA

## Project Overview

This project performs a complete Exploratory Data Analysis (EDA) on a road accident dataset containing accident, driver, vehicle, weather, road, and emergency response information.

The objective is to identify accident patterns, severity factors, temporal trends, and risk indicators that contribute to road accidents. The project follows a structured EDA workflow including data cleaning, preprocessing, statistical testing, feature engineering, and visualization.

---

## Dataset Description

### Dataset Characteristics

* Total Records: 5,700+
* Features: 20+ columns
* Numerical Variables
* Categorical Variables
* Date and Time Variables

### Key Features

| Column                      | Description                 |
| --------------------------- | --------------------------- |
| Accident_ID                 | Unique accident identifier  |
| Accident_Date               | Date of accident            |
| Accident_Hour               | Hour of accident occurrence |
| District                    | Accident location district  |
| Road_Type                   | Type of road                |
| Weather_Condition           | Weather during accident     |
| Vehicle_Type                | Vehicle involved            |
| Driver_Age                  | Driver age                  |
| Driver_Gender               | Driver gender               |
| Alcohol_Involved            | Alcohol involvement status  |
| Vehicle_Speed_kmph          | Vehicle speed               |
| Helmet_Used                 | Helmet usage status         |
| Seatbelt_Used               | Seatbelt usage status       |
| Accident_Severity           | Severity of accident        |
| Casualties_Count            | Number of casualties        |
| Injury_Type                 | Type of injury              |
| Emergency_Response_Time_Min | Emergency response time     |

---

## Project Objectives

* Understand the dataset structure and quality
* Handle missing values and duplicates
* Detect and treat outliers
* Perform univariate and bivariate analysis
* Conduct statistical hypothesis testing
* Analyze accident trends over time
* Engineer meaningful features
* Generate actionable insights from the data

---

## Project Workflow

### Day 1 – Data Understanding & Profiling

* Dataset overview
* Data type inspection
* Missing value analysis
* Data quality assessment

Notebook:
`01_data_overview.ipynb`

---

### Day 2 – Data Cleaning & Preprocessing

* Datatype corrections
* Missing value treatment
* Duplicate removal
* Outlier detection and handling
* Data standardization

Notebook:
`02_cleaning_preprocessing.ipynb`

Output:
`data/interim/cleaned_day2.csv`

---

### Day 3 – Univariate & Bivariate EDA

* Distribution analysis
* Correlation analysis
* Categorical analysis
* Segment analysis
* Visualization generation

Notebook:
`03_univariate_bivariate_eda.ipynb`

Figures:
`reports/figures/`

---

### Day 4 – Statistical Tests, Time EDA & Feature Engineering

* T-Test
* ANOVA
* Chi-Square Test
* Time-based analysis
* Feature engineering
* Risk factor analysis

Notebook:
`04_stats_time_features_final_insights.ipynb`

Output:
`data/processed/final_cleaned_day4.csv`

---

## Feature Engineering

The following features were created:

* Accident_Year
* Accident_Month
* Day_Of_Week
* Is_Weekend
* Time_Block
* Age_Group
* High_Speed
* Delayed_Response
* Night_Driving
* Multiple_Casualties

---

## Statistical Tests Performed

### Independent T-Test

Used to compare vehicle speeds between fatal and minor accidents.

### ANOVA

Used to determine whether emergency response times differ across road types.

### Chi-Square Test

Used to analyze the relationship between helmet usage and accident severity.

---

## Key Insights

* Accident frequency varies across different months and weekdays.
* Certain districts experience a higher number of accidents.
* Vehicle speed shows a relationship with accident severity.
* Alcohol involvement contributes to accident severity patterns.
* Helmet and seatbelt usage are associated with safer outcomes.
* Emergency response times vary across road types.
* Night-time accidents exhibit different severity characteristics compared to daytime accidents.
* Driver age groups show different accident involvement patterns.

---

## Project Structure

```text
Road-Accident-EDA/
│
├── data/
│   ├── raw/
│   ├── interim/
│   └── processed/
│
├── notebooks/
│   ├── 01_data_overview.ipynb
│   ├── 02_cleaning_preprocessing.ipynb
│   ├── 03_univariate_bivariate_eda.ipynb
│   └── 04_stats_time_features_final_insights.ipynb
│
├── reports/
│   └── figures/
│
├── .gitignore
├── README.md
└── requirements.txt
```

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy
* Jupyter Notebook
* Git
* GitHub

---

## How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/AswinSanthoshDev/Road-Accident-EDA.git
```

### 2. Navigate to Project Folder

```bash
cd Road-Accident-EDA
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run Notebooks

Execute notebooks in the following order:

1. 01_data_overview.ipynb
2. 02_cleaning_preprocessing.ipynb
3. 03_univariate_bivariate_eda.ipynb
4. 04_stats_time_features_final_insights.ipynb

---

## Author

**Aswin Santhosh**

GitHub: https://github.com/AswinSanthoshDev

