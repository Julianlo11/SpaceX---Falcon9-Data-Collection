# 🚀 SpaceX Falcon 9 – Data Collection and Data Wrangling

## 📌 Project Overview

This project is part of the **SpaceX Falcon 9 First Stage Landing Prediction** laboratory, developed as part of my Data Science and Machine Learning training.

The main objective is to collect, explore, clean, and prepare historical SpaceX launch data, focusing on Falcon 9 rockets. This work establishes the foundation for analyzing the factors that influence the successful landing of the rocket's first stage.

## 🎯 Project Objectives

- Collect launch data using the SpaceX API.
- Transform JSON responses into structured DataFrames.
- Explore and analyze historical launch information.
- Filter Falcon 9 launch records.
- Identify and handle missing values.
- Prepare datasets for subsequent data analysis and Machine Learning tasks.

## 🛠️ Technologies and Tools

| Technology | Application |
|---|---|
| Python | Programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Missing value treatment |
| Requests | API requests |
| Matplotlib | Data visualization |
| Jupyter Notebook | Development and documentation |

## 📊 Project Development

### Task 1 – Collecting the Data

- Retrieved SpaceX launch information using HTTP GET requests.
- Processed JSON responses from the SpaceX API.
- Converted JSON data into Pandas DataFrames using `pd.json_normalize()`.
- Selected relevant variables, including rocket, payload, launchpad, flight number, and launch date.
- Explored a historical dataset provided by IBM Skills Network to support the analysis.

### Task 2 – Filtering Falcon 9 Launches

Filtered the launch records to focus exclusively on Falcon 9 rockets and performed data validation.

**Key results:**

| Metric | Result |
|---|---:|
| Falcon 9 launches | 90 |
| Unique flight numbers | 90 |
| Duplicate flight numbers | 0 |
| Unique payload records | 90 |
| Unique launch dates | 90 |
| Launch platforms | 3 |
| Missing values in API dataset | 0 |

**Launch distribution by platform:**

| Launch Platform ID | Launches | Percentage |
|---|---:|---:|
| Platform 1 | 55 | 61.11% |
| Platform 2 | 22 | 24.44% |
| Platform 3 | 13 | 14.44% |

Additional exploratory analysis included launch frequency by year, orbit distribution, landing outcomes, and descriptive statistics.

### Task 3 – Dealing with Missing Values

Performed missing value analysis and data preparation using the historical IBM dataset.

Activities included:

- Identifying missing values using `isnull()` and `sum()`.
- Calculating the average payload mass using `.mean()`.
- Replacing missing values with NumPy and Pandas `.replace()`.
- Validating the results after treatment.
- Exporting the prepared dataset to CSV format.

**Results:**

| Metric | Result |
|---|---:|
| Total records | 90 |
| Total columns | 17 |
| Average Payload Mass | 6,104.96 kg |
| Missing values in PayloadMass | 0 |
| Missing values in LandingPad | 26 |

The missing values in `LandingPad` were preserved because they represent unavailable or non-applicable landing platform information.

## 📁 Project Structure

```text
SpaceX-Falcon9-Data-Collection/
│
├── jupyter-labs-spacex-data-collection-api.ipynb
├── dataset_part_1.csv
└── README.md
```

## 📈 Key Findings

- A total of 90 Falcon 9 launches were identified in the filtered API dataset.
- One launch platform accounted for approximately 61.11% of the recorded launches.
- The historical dataset provided an average payload mass of approximately 6,104.96 kg.
- Data validation and missing value treatment were performed to prepare the dataset for further analysis.

## 🧠 Skills Developed

- Data Collection and API Integration
- Exploratory Data Analysis (EDA)
- Data Cleaning and Preprocessing
- Data Manipulation with Pandas
- Missing Value Treatment
- Data Visualization
- Python Programming
- Data Validation

## 📚 Data Sources

- [SpaceX API](https://api.spacexdata.com/v4/launches/past)
- [IBM Skills Network – Historical SpaceX Dataset](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DS0321EN-SkillsNetwork/datasets/dataset_part_1.csv)
- [IBM Skills Network – SpaceX API Static Dataset](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DS0321EN-SkillsNetwork/datasets/API_call_spacex_api.json)

## 📝 Conclusion

This laboratory provided practical experience in the initial stages of a Data Science project, covering data collection, exploration, cleaning, validation, and preparation.

Through Python, Pandas, NumPy, and Matplotlib, I developed practical skills in transforming raw information into structured datasets suitable for further analysis.

This project represents the foundation for the next stages of the SpaceX Falcon 9 First Stage Landing Prediction project, where statistical analysis and Machine Learning techniques will be applied to investigate the factors associated with successful first-stage landings.

## 👨‍💻 Author

**Julian Daniel Lopez Cano**

Economist | Data Science & Machine Learning

Interested in Data Analytics, Business Intelligence, Python, SQL, and Machine Learning.

[GitHub – Julianlo11](https://github.com/Julianlo11)