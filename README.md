# Smart City Traffic Pattern Forecasting

## 📌 Project Overview
This project focuses on analyzing and forecasting traffic patterns at multiple city junctions as part of a smart city initiative. Using historical traffic data, the project aims to understand temporal traffic behavior and predict future traffic volumes to support proactive traffic management and infrastructure planning.

## 🎯 Problem Statement
Urban traffic congestion is a major challenge in smart city development. Traffic patterns vary across different junctions and change over time based on working days, weekends, and special occasions. The objective of this project is to analyze traffic data from four city junctions and forecast future traffic volumes so that government authorities can prepare for traffic peaks in advance.

## 📊 Dataset Description
The project uses two datasets:
- **Training Dataset:** Contains historical traffic data with the following columns:
  - DateTime: Timestamp of traffic observation
  - Junction: Junction identifier
  - Vehicles: Number of vehicles (target variable)
- **Testing Dataset:** Contains future timestamps and junction information without the target variable.

The datasets represent time-series traffic data collected from four different junctions.

## 🔍 Exploratory Data Analysis (EDA)
EDA was performed on the training dataset to understand traffic behavior and patterns. The following analyses were conducted:
- Traffic volume distribution analysis
- Traffic trends over time
- Junction-wise traffic comparison
- Hourly traffic pattern analysis
- Day-of-week traffic variation

These analyses helped identify peak hours, high-traffic junctions, and temporal variations in traffic flow.

## ⚙️ Feature Engineering
To capture time-based traffic patterns, the following features were extracted from the DateTime column:
- Hour of the day
- Day of the week
- Month
- Weekend indicator

These features enabled the model to learn daily and weekly traffic trends effectively.

## 🧠 Models Implemented
The following machine learning models were implemented and compared:
- **Linear Regression:** Used as a baseline model
- **Random Forest Regressor:** Used to capture non-linear traffic patterns

## 📈 Model Evaluation
Models were evaluated using standard regression metrics:
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

Random Forest Regressor outperformed Linear Regression by achieving lower error values and a higher R² score, indicating better predictive performance.

## 🚦 Traffic Forecasting
The final Random Forest model was trained on the complete training dataset and used to forecast traffic volumes for the test dataset. Forecasted results were visualized over time and across
