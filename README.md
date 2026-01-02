# Fuel Usage Data Cleaning and Exploratory Analysis

This repository contains a data science project focused on cleaning, exploring, and analysing a large-scale, real-world fuel usage dataset.  
The dataset consists of user-submitted fuel logs collected globally and is highly noisy, inconsistent, and incomplete.

The project was completed as part of a Data Visualization and Exploration course, with an emphasis on critical data reasoning rather than purely technical execution.

---

## 📊 Project Overview

The primary goals of this project were to:
- Clean and standardise a messy, user-generated dataset
- Engineer meaningful features from raw string-based inputs
- Identify and remove implausible values using domain knowledge
- Explore fuel usage, vehicle characteristics, and refuelling behaviour across countries
- Extract realistic insights despite high data noise

The dataset includes information such as fueling dates, odometer readings, fuel volumes, costs, currencies, vehicle details, and user activity.

---

## 🧹 Data Cleaning and Feature Engineering

Key steps included:
- Parsing and repairing corrupted date fields
- Converting numeric fields stored as strings (with commas and symbols) into usable floats
- Reconstructing missing values using interdependent relationships (miles, gallons, MPG)
- Extracting currency, vehicle make, model, year, and user ID from URLs
- Converting imperial units to metric (litres, kilometres, L/100km)
- Applying domain-informed thresholds to remove implausible outliers

After cleaning and filtering, approximately 27% of records were removed to ensure realistic analysis.

---

## 🔍 Exploratory Analysis Highlights

The analysis explored:
- Global usage patterns of the fuel logging application
- Vehicle age distributions across countries
- Popular vehicle makes and models
- Fuel efficiency comparisons between regions
- Seasonal fuel efficiency differences
- Strategic refuelling behaviour in South Africa around monthly fuel price changes

Notably, the results show strong evidence of strategic consumer behaviour in South Africa, with significantly increased refuelling activity on Tuesdays prior to fuel price increases.

---

## 🤖 Modelling

A Random Forest regressor was used to analyse feature importance for fuel efficiency.  
The model largely rediscovered the mathematical relationship between fuel consumed and distance travelled, highlighting the limitations of predictive modelling on derived variables and noisy user-generated data.

---

## 🧠 Key Takeaways

- Real-world datasets often require aggressive cleaning and careful reasoning before analysis
- Domain knowledge is essential for identifying implausible values
- Apparent statistical relationships must be interpreted cautiously when variables are derived
- Despite noise, meaningful behavioural and regional insights can still be extracted

---

## 👥 Collaboration

This project was completed collaboratively.

My contributions focused on:
- Data cleaning and type conversion
- Feature engineering
- Outlier detection and justification
- Statistical analysis and interpretation
- Writing and structuring the final report

The full academic report is available in the `report/` directory.
