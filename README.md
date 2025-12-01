# 🌡️ Weather Temperature Prediction Using OLS Regression

This project demonstrates **predicting daily temperatures** using historical weather data.  
It applies **Ordinary Least Squares (OLS) regression** to model temperature based on multiple meteorological features and evaluates feature significance with **statistical hypothesis testing**.

---

## 📂 Project Structure

- **weatherHistory.csv**   
- **Temperature_Prediction_OLS_Regression_&_Hypothesis_Testing_by_Kadasani_Bhuvana_Reddy_24XV1M0518.ipynb** 
- **README.md**

  
## 🔍 Overview

The dataset contains weather measurements like temperature, humidity, wind speed, and precipitation type.  
The main goal is to **predict the actual temperature (`Temp`)** using these predictors and understand how each feature influences it.

---

## 🛠️ Tools & Libraries

This project uses the following **Python libraries** and **tools**:

- **Python 3.x** – Programming language  
- **Jupyter Notebook / Google Colab** – Notebook environment for interactive analysis  
- **Pandas** – Data manipulation and preprocessing  
- **NumPy** – Numerical computations  
- **Matplotlib & Seaborn** – Data visualization  
- **Scikit-learn** – Label encoding for categorical features  
- **Statsmodels** – OLS regression and statistical analysis  
- **SciPy** – Statistical tests (chi-square, z-test)

---


## 📋 Dataset Features

| Feature          | Description |
|-----------------|-------------|
| PrecipType       | Type of precipitation (rain, snow) |
| AppTemp          | Apparent temperature in Celsius |
| Humidity         | Relative humidity (%) |
| WindSpeed        | Wind speed in km/h |
| WindBearing      | Wind direction (degrees) |
| Visibility       | Visibility distance in km |
| Pressure         | Atmospheric pressure (millibars) |
| year             | Year of observation |
| month            | Month of observation |
| day              | Day of observation |

**Target Variable:** `Temp` (Temperature in °C)

---

## 🚀 Objectives

- Build an OLS regression model to predict temperature  
- Identify which features significantly impact temperature  
- Analyze relationships between temperature and other weather variables  
- Apply t-tests, z-tests, and chi-square tests to validate feature contributions  

---

## ⚙️ Project Workflow

1. **Data Preprocessing**
   - Load dataset and handle missing values  
   - Extract `year`, `month`, `day` from timestamp  
   - Remove duplicates and unnecessary columns  
   - Encode categorical variables for modeling  

2. **Exploratory Data Analysis**
   - Visualize correlations between features  
   - Highlight features most associated with temperature  

3. **OLS Regression**
   - Fit a linear regression model using all predictors  
   - Inspect coefficients, R² score, and p-values  
   - Plot actual vs predicted temperatures to assess model performance  

4. **Hypothesis Testing**
   - **t-test:** Check significance of individual regression coefficients  
   - **Z-test:** Approximation to confirm coefficient relevance  
   - **Chi-square test:** Evaluate dependency between discretized temperature and apparent temperature  

---

## 📊 Key Insights

- **AppTemp** is the strongest predictor of actual temperature  
- Meteorological variables like **Humidity, WindSpeed, Visibility, and Pressure** moderately influence temperature  
- **Precipitation type** significantly affects temperature patterns  
- Temporal variables (`year`, `month`, `day`) capture seasonal and long-term trends  
- All predictors were statistically significant in the OLS model (p < 0.05)  
- Chi-square test confirms that discretized temperature and apparent temperature are highly dependent  

---


## 📈 How to Use

1. Clone the repository and open the notebook in **Google Colab** or **Jupyter Notebook**  
2. Upload the `weatherHistory.csv` dataset to `data/` folder  
3. Execute cells in the notebook sequentially to perform:
   - Data preprocessing  
   - Regression modeling  
   - Hypothesis testing and analysis  
   - Visualization of actual vs predicted temperature


## 🔹 Conclusion

The OLS regression model effectively predicts temperature using multiple meteorological features.  
Statistical tests validate that each feature contributes meaningful information.  
Seasonal, temporal, and weather-related variables all play a role in shaping daily temperature patterns.

##  Author

Created by **Kadasani Bhuvana Reddy**
