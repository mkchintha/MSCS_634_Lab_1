## Author
Murali Krishna Chintha

## Course
MSCS-634-M40 – Advanced Big Data and Data Mining

## Assignment
Lab 1 – Data Visualization, Data Preprocessing, and Statistical Analysis Using Python in Jupyter Notebook

---

## Purpose
This lab demonstrates the application of data preprocessing, visualization, and statistical analysis techniques on a real-world weather dataset (`weatherAUS.csv`). The goal is to explore the data, clean it, visualize relationships, and derive meaningful insights using Python and Jupyter Notebook.

---

## Steps Completed

### ✅ Step 1: Data Collection
- Loaded the dataset into a Pandas DataFrame.
- Displayed the first few rows for initial inspection.

### 📊 Step 2: Data Visualization
- **Heatmap** to identify missing values across columns.
- **Scatter plot** to explore the relationship between `MinTemp` and `MaxTemp`.
- **Histogram** to examine the distribution of `Rainfall`.
- **Box plot** to detect outliers in `Rainfall`.
- **Bar plot** for frequency of `RainToday`.
- **Line plot** of `Temp3pm` over time for the Albury location.
- **Pairplot** of `MinTemp`, `MaxTemp`, `Temp3pm`, and `Humidity3pm`.
- **Boxplot by location** for `Rainfall`.
- **Violin plot** for `Temp3pm` grouped by `RainToday`.
- **Lineplot** for average `MaxTemp` trend over time.

### 🧹 Step 3: Data Preprocessing
- **Missing values** handled using mean imputation for numerical features.
- **Outlier detection and removal** performed on `Rainfall` using IQR method.
- **Data reduction** done by dropping `Evaporation` and `Sunshine` due to high null values.
- **Min-Max Scaling** applied to normalize `MinTemp`, `MaxTemp`, and `Rainfall`.

### 📈 Step 4: Statistical Analysis
- Displayed `.info()` and `.describe()` to understand dataset structure and summary statistics.
- Calculated central tendency: min, max, mean, median, and mode.
- Computed dispersion measures: range, variance, and standard deviation.
- Evaluated **skewness** and **kurtosis** for data shape understanding.
- Generated **covariance** and **correlation matrices** to study relationships.
- Analyzed frequency distribution for categorical variable `RainToday`.

---

## Key Insights
- Rainfall is highly skewed and exhibits heavy tails, with many dry days and few extreme rain events.
- Strong correlation observed between `MinTemp` and `MaxTemp`.
- Negative correlation between humidity and temperature supports expected weather behavior.
- Outlier handling significantly improved `Rainfall` distribution.
- Cloud coverage and pressure data are moderately balanced and skew-resistant.
- Temperature and rainfall distributions became well-suited for analysis after scaling.
- Rainfall distribution is highly right-skewed, with a skewness of 2.61, indicating that most days are dry with occasional extreme rain events.
- Rainfall also exhibits high kurtosis (5.78), confirming the presence of heavy tails and extreme outliers even after IQR filtering.
- Humidity at 9am is negatively correlated with temperature, suggesting that cooler mornings tend to have higher humidity levels.
- MinTemp and MaxTemp are strongly positively correlated, reflecting expected daily temperature patterns.
- Wind speeds and gusts show moderate positive correlation with rainfall, implying windier conditions may coincide with rainy days.
- Cloud coverage (Cloud9am/Cloud3pm) shows mild left skew, meaning most days are partly to fully cloudy.
- Most numerical features such as temperature and pressure exhibit near-normal distributions after scaling, supporting the suitability for further statistical modeling.

---

## Challenges
- Several columns had high missing values, requiring thoughtful imputation or removal.
- Rainfall and weather conditions vary widely across different locations.
- Careful visualization was needed to explore and present data effectively.

---

## Screenshots
All screenshots required for lab submission are available in the `/screenshots/` folder.

---

## Dataset Source
The dataset is uploaded in the `/dataset/` folder, also can be found in below link:
[weatherAUS.csv – Kaggle](https://www.kaggle.com/jsphyg/weather-dataset-rattle-package)

---

## Notes
This notebook is designed to showcase practical data science workflow using Python: from data loading, cleaning, visualization, to deriving statistical insights. It lays a strong foundation for future data modeling and predictive analytics work.
