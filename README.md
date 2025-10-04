# 🚜 Bulldozer Auction Price Prediction  

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg) ![Scikit-Learn](https://img.shields.io/badge/ML-ScikitLearn-orange)  ![Random Forest](https://img.shields.io/badge/Algorithm-RandomForest-green) ![R² Score](https://img.shields.io/badge/R²-0.88-brightgreen)  ![MAE](https://img.shields.io/badge/MAE-5951-lightblue)  

---

## 📌 Table of Contents
- [Project Overview](#-project-overview)  
- [Dataset](#-dataset)  
- [Features](#-features)  
- [Project Workflow](#-project-workflow)  
- [Project Deliverables](#-project-deliverables)  
- [Key Learnings](#-key-learnings)  
- [Results](#-results)  
- [Tools & Technologies Used](#-tools--technologies-used)  
- [Skills Demonstrated](#%E2%80%8D-skills-demonstrated)  
- [Connect with Me](#-connect-with-me)  

---

## 🚀 Project Overview  

This project focuses on **predicting the future sale prices of bulldozers at auction** using **real-world industrial auction data**.  
The dataset contains **400,000+ records** of historical bulldozer sales, making it one of the most comprehensive real-world regression problems on Kaggle.  

The model helps equipment dealers, auctioneers, and analysts make **data-driven pricing decisions** by analyzing features such as **year of manufacture, machine type, usage, and auctioneer details**.  

---

## 📂 Dataset  

**Source:** [Kaggle - Blue Book for Bulldozers](https://www.kaggle.com/c/bluebook-for-bulldozers)  

- **Size:** 400K+ records of bulldozer auctions 📊  
- **Train.csv** → Data until end of 2011  
- **Valid.csv** → Data from Jan 2012 – Apr 2012  
- **Test.csv** → Data from May 2012 – Nov 2012 (final evaluation set)  

This large-scale dataset simulates a **real-world pricing challenge** where accurate predictions can significantly impact business profitability.  

---

## 🔑 Features  

Some key attributes used for prediction:  
- **SalesID, MachineID, ModelID** – Identifiers  
- **YearMade** – Manufacturing year  
- **MachineHoursCurrentMeter** – Usage in hours  
- **UsageBand** – Low / Medium / High usage  
- **ProductClassDesc, State, AuctioneerID** – Categorical details  
- **Saledate** – Date of sale  
- **SalePrice (target)** – Bulldozer price in USD  

---

## 🛠 Project Workflow  

**Exploratory Data Analysis (EDA) 🔍**  
- Checked missing values and feature distributions  
- Identified categorical vs numerical features  

**Data Preprocessing 🧹**  
- Filled missing values  
- Encoded categorical variables  
- Extracted useful date-time features  

**Feature Engineering ⚙️**  
- Added machine age, usage metrics  
- Derived year-based temporal features  

**Model Training 🤖**  
- Baseline Model (Dummy Regressor) for reference  
- Random Forest Regressor as main model  
- Hyperparameter tuning using **RandomizedSearchCV**  

**Evaluation Metrics 📊**  
- R² Score  
- Mean Absolute Error (MAE)  
- Root Mean Squared Log Error (RMSLE)  

---

## 📦 Project Deliverables  

This repository contains:  
- Jupyter Notebook (`Bulldozer_Price_Prediction.ipynb`) 📒  
- Training & Validation Data (from Kaggle) 📂  
- Preprocessing & Feature Engineering pipeline ⚙️  
- Trained ML Model (Random Forest) 🌲  

---

## 🎯 Key Learnings  
- Importance of handling **missing values** and **categorical encodings** in ML pipelines.  
- **Feature engineering** (temporal features like year, month, machine age) significantly boosts model accuracy.  
- **Random Forest Regressor with hyperparameter tuning** improves generalization and reduces errors.  
- Choosing **domain-appropriate metrics** (RMSLE > RMSE for price predictions) is crucial.  
- Working with **large-scale real-world datasets (400K+ records)** requires efficient memory and computation handling.  

---

## 📈 Results  

- ✅ **Training R²** = 95.88%  
- ✅ **Validation R²** = 88.18%  
- ✅ **Training MAE** = 2953.82  
- ✅ **Validation MAE** = 5951.25  
- ✅ **Training RMSLE** = 0.1447  
- ✅ **Validation RMSLE** = 0.2452  

📉  Reduced pricing errors by ~70% compared to a baseline model, and analyzed feature importance to identify key price drivers, guiding profitable auction strategies.

---

### 🔹 Project Results  (Based on Validation Dataset: Year 2012)

### 🔹 Project Results (Validation Dataset: Year 2012)

<table>
  <tr>
    <td align="center">
      <img src="Project Visuals/Feature Importance.png" alt="Feature Importance" width="280"/><br/>
      <b>Feature Importance</b><br/>
      Key factors affecting bulldozer prices are the year made, product size, and year of sale.
    </td>
    <td align="center">
      <img src="Project Visuals/Actual Sale Price vs Predicted Sale Price.png" alt="Actual vs Predicted" width="280"/><br/>
      <b>Actual vs Predicted Prices</b><br/>
      On the 2012 validation set, predictions align closely with actual auction prices, showing strong accuracy.
    </td>
    <td align="center">
      <img src="Project Visuals/Distribution of Predicted Errors.png" alt="Residuals Distribution" width="280"/><br/>
      <b>Error Distribution</b><br/>
      Most prediction errors are small and centered around zero, meaning the model is stable and reliable.
    </td>
  </tr>
</table>

---

## 🛠 Tools & Technologies Used  
- **Python** 🐍  
- **Pandas, NumPy** for data handling  
- **Matplotlib, Seaborn** for visualization  
- **Scikit-learn** for ML modeling  
- **Jupyter Notebook** for experimentation  

---

## 🧑‍💻 Skills Demonstrated  
- Data Cleaning & Preprocessing  
- Exploratory Data Analysis (EDA)  
- Feature Engineering  
- Model Training & Evaluation  
- Hyperparameter Tuning  
- Business Insight Generation  
- Working with **large real-world datasets (400K+ rows)**  

---

## 🤝 Connect with Me  
📌 GitHub: [Check Out my GitHub Profile for other Projects](https://github.com/noumanjamadar/)  
💼 LinkedIn: [Mohammad Navaman Jamadar](https://www.linkedin.com/in/mohammad-navaman-jamadar/)  

