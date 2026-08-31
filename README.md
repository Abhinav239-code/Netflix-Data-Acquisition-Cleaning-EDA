# Netflix Data Acquisition, Cleaning & Exploratory Data Analysis

## 📌 Project Overview

This project demonstrates the complete data preparation and exploratory data analysis workflow using the Netflix Movies and TV Shows dataset.

The project focuses on:

* Data Acquisition
* Data Understanding
* Data Cleaning
* Missing Value Analysis
* Duplicate Removal
* Data Type Correction
* Exploratory Data Analysis
* Data Visualization
* Insight Generation

## 🎯 Objectives

The main objectives of this project are:

1. Acquire a publicly available Netflix dataset.
2. Understand the structure and characteristics of the dataset.
3. Identify and handle missing values.
4. Detect and remove duplicate records.
5. Correct inappropriate data types.
6. Perform exploratory data analysis.
7. Create meaningful visualizations.
8. Extract useful insights from the dataset.

## 📊 Dataset

**Dataset:** Netflix Movies and TV Shows

**Source:** Kaggle

[Netflix Movies and TV Shows Dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows)

The dataset contains information about movies and TV shows available on Netflix, including:

* Type
* Title
* Director
* Cast
* Country
* Release Year
* Rating
* Duration
* Date Added
* Listed In

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook
* GitHub

## 🧹 Data Cleaning

The following preprocessing operations were performed:

### Missing Values

Missing values were identified using:

```python
df.isnull().sum()
```

Categorical missing values were handled appropriately instead of unnecessarily deleting records.

### Duplicate Records

Duplicate records were identified using:

```python
df.duplicated().sum()
```

and removed using:

```python
df = df.drop_duplicates()
```

### Data Type Correction

Relevant numerical and date columns were converted into appropriate data types.

## 📈 Exploratory Data Analysis

The following analyses were performed:

* Movies vs TV Shows
* Missing Value Analysis
* Release Year Analysis
* Movie Duration Distribution
* Country-wise Content Analysis
* Correlation Analysis

## 📊 Visualizations

### Movies vs TV Shows

![Movies vs TV Shows](visualizations/content_type.png)

### Missing Values

![Missing Values](visualizations/missing_values.png)

### Release Year Analysis

![Release Year](visualizations/release_year.png)

### Movie Duration

![Movie Duration](visualizations/duration.png)

### Country Analysis

![Countries](visualizations/countries.png)

### Correlation Analysis

![Correlation](visualizations/correlation.png)

## 🔍 Key Insights

* Movies represent a major portion of the Netflix content catalog.
* Missing values occur in several columns and need to be handled carefully.
* Some missing values are naturally associated with fields that are not applicable to a particular content type.
* Release year provides useful information for studying content trends.
* Movie duration is concentrated around typical feature-film lengths.
* Country is an important variable for geographical content analysis.

## 📁 Project Structure

```text
Netflix-Data-Acquisition-Cleaning-EDA/
│
├── data/
│   └── netflix_titles.csv
│
├── notebooks/
│   └── Netflix_EDA.ipynb
│
├── visualizations/
│   ├── missing_values.png
│   ├── content_type.png
│   ├── release_year.png
│   ├── duration.png
│   ├── countries.png
│   └── correlation.png
│
├── report/
│   └── Week_1_Data_Acquisition_Cleaning_EDA_Report.docx
│
├── README.md
│
└── requirements.txt
```

## 🚀 Future Scope

Future work can include:

* Netflix content recommendation system
* Country-wise content comparison
* Content trend prediction
* Rating analysis
* Machine learning-based recommendation
* Interactive dashboard using Power BI or Streamlit

## 👨‍💻 Author

**Abhinav Sharma**

B.Tech – CSE (Data Science)

## 📄 License

This project uses a publicly available dataset from Kaggle.
