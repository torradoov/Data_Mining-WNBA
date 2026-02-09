# WNBA Pre-Season Prediction System 🏀

This project was developed for the **Data Mining** course at the **Faculty of Engineering of the University of Porto (FEUP)** by **Group 76**.

## 📋 Overview
The primary goal of this system is to support strategic decision-making during the WNBA pre-season through data-driven predictions. A key constraint of this project is that all predictions are made strictly before the season begins, without utilizing any data or statistics from the target year.

## 🎯 Project Objectives
The project is divided into three main predictive pillars:
1.  **Conference Rankings:** Predicting final standings for both conferences using historical team-level data.
2.  **Coach Turnover:** Identifying teams with a high probability of changing their head coach based on past performance trends.
3.  **Individual Awards:** Predicting winners for major individual awards (e.g., MVP, Rookie of the Year) using player performance metrics.

## 🛠️ Modeling Strategy
Each objective was addressed using a task-specific Machine Learning approach to handle different data structures and targets:
* **Rankings:** Modeled using **Random Forest** (East Conference) and **Linear Regression** (West Conference).
* **Coaching Changes:** Implemented via a **Soft Voting Ensemble** (combining Logistic Regression, Random Forest, and Gradient Boosting).
* **Awards:** Utilized a **Random Forest Classifier** to address the significant class imbalance (only one winner per award).

## 📊 Dataset
The models were trained on a dataset spanning 10 WNBA seasons, including:
* **Teams & Coaches:** Historical records and management changes.
* **Player Performance:** Detailed box scores and individual statistics.
* **Post-season & Awards:** Results from previous playoffs and honors.

## ⚠️ Limitations & Future Work
* **Data Skewness:** Historical data is naturally skewed (varying number of games and rare events).
* **Human Factors:** Models cannot account for mid-season injuries, trades, or team chemistry.
* **Future Work:** Transitioning from static pre-season predictions to dynamic weekly updates and integrating external data (News/Social Media) to capture fan and management pressure.

---
**Authors (Group 76):**
* Diogo Neves
* Pedro Paixão
* Tiago Torrado
