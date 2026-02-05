# Delhi-Outdoor-Safety-Prediction-System
A machine learning–based public health decision system that predicts whether it is safe to go outdoors in Delhi using live air quality and meteorological data from OpenWeather, NASA, and OpenAQ APIs.

# **🌍 Delhi Outdoor Safety Prediction System**
Machine Learning–Driven Public Health Decision Framework

**📌 Project Overview**

Delhi frequently experiences severe air pollution due to vehicle emissions, industrial activities, construction dust, and unfavorable weather conditions. Prolonged exposure to polluted air poses serious health risks, especially for children, elderly citizens, and individuals with respiratory or cardiovascular conditions.

This project aims to build a machine learning–based decision system that predicts whether it is safe to go outdoors tomorrow based on recent air quality and meteorological conditions.
The system leverages live environmental APIs, historical trends, and data-driven insights to support preventive public health decisions.

### **🎯 Objective**

To classify outdoor safety for the next day into a binary outcome:

✅ YES – It is reasonably safe to go outdoors

❌ NO – Outdoor exposure should be avoided due to health risks

This prediction helps citizens, healthcare authorities, and policymakers take proactive action instead of reacting after health damage occurs.

### **🧠 Problem Domain**

-Environmental Analytics

- Public Health & Safety

- Smart Cities

- Applied Machine Learning

- Real-Time Data Engineering

### **📊 Data Sources (Live APIs)**

- This project exclusively uses free and open-source APIs for real-world applicability:

- OpenWeather API – Air pollution and meteorological data

- NASA POWER API – Historical weather parameters

- OpenAQ – Air quality monitoring data

- All data is fetched programmatically and processed automatically.

### **🧩 Feature Schema**
🌦 Meteorological Features
| Feature                    | Description                                           |
| -------------------------- | ----------------------------------------------------- |
| Temperature (°C)           | Influences pollutant reactions and human comfort      |
| Humidity (%)               | Affects particulate suspension and respiratory stress |
| Wind Speed (m/s)           | Determines pollutant dispersion or accumulation       |
| Atmospheric Pressure (hPa) | Impacts air stagnation and pollution buildup          |
| Rainfall (mm)              | Acts as a natural pollutant washout mechanism         |

### **🌫 Air Pollution Features**
| Feature       | Description                                          |
| ------------- | ---------------------------------------------------- |
| PM2.5 (μg/m³) | Fine particles penetrating deep into lungs           |
| PM10 (μg/m³)  | Causes airway irritation                             |
| CO (μg/m³)    | Reduces oxygen-carrying capacity of blood            |
| NO₂ (μg/m³)   | Traffic-related pollutant affecting lung function    |
| SO₂ (μg/m³)   | Industrial pollutant causing bronchial irritation    |
| O₃ (μg/m³)    | Ground-level ozone causing breathing difficulty      |
| AQI           | Aggregated measure of overall air pollution severity |

### **🔍 Exploratory Data Analysis (EDA)**

- Identified pollution trends over time

- Analyzed correlation between meteorological and pollution features

- Detected seasonal and stagnation patterns

- Studied impact of wind speed and rainfall on AQI levels

- Outlier detection using box plots and distributions

### **🛠 Feature Engineering**

- Key engineered features include:

- Time-based features (day, month, weekday, weekend)

- Lag features (previous day AQI and pollutant levels)

- Rolling averages (3-day and 7-day trends)

- Ratio features (PM2.5 / PM10, NO₂ / SO₂)

- Interaction features (pollutants × weather)

- Binary Outdoor Safety Label derived from AQI thresholds

### **🤖 Model Selection**

- The problem is framed as a binary classification task.

**Selected Model:**

- Random Forest Classifier

**Why Random Forest?**

- Handles non-linear relationships effectively

- Robust to noise and outliers

- No strict feature scaling required

- Works well with tabular environmental data

- Provides feature importance insights

### **📈 Model Performance**

- Train Accuracy: ~90%

- Test Accuracy: ~100%

- High performance indicates strong pattern learning from environmental trends. Model validation techniques were applied to minimize overfitting risk.

### **⏳ Prediction Workflow**

- Fetch latest live environmental data

- Apply feature engineering pipeline

- Feed processed data into trained model

- Predict Outdoor Safety for Tomorrow

### **📢 Output:**

Tomorrow Outdoor Safety Prediction: YES / NO

### **🚀 Future Enhancements**

- Hourly-level forecasting for time-specific safety alerts

- Multi-day pollution forecasting

- Mobile app or web dashboard deployment

- Integration with health advisory systems

- City-wide scalability beyond Delhi

### **🧑‍💻 Tech Stack**

Python

Pandas, NumPy

Scikit-learn

Plotly & Matplotlib

REST APIs

Jupyter Notebook / VS Code


### **🏁 Conclusion**

This project demonstrates how machine learning combined with live environmental data can support real-world public health decisions.
By predicting outdoor safety proactively, the system helps reduce health risks and supports smarter, healthier urban living.
