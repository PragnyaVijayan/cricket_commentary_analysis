# Unveiling Cricket Dynamics: Extracting Insights from Ball-By-Ball Data

## Overview
This project analyzes ball-by-ball cricket data from the 2022 T20 Asia Cup to extract meaningful insights and predict player performance using data visualization and predictive modeling techniques. The goal is to compare team and player statistics and build predictive models to assess player effectiveness. The project uses web-scraped data from ESPN Cricinfo and interactive data visualization with Dash, a Python framework for web applications.

## Authors
- **Pragnya Vijayan**
- **Vignesh Senthilkumar**

## Dataset
- **Source**: The dataset was collected via web scraping from ESPN Cricinfo and is available on Kaggle.
- **Modifications**:
  - Added missing feature columns (bowling team, winning team).
  - Used regex to clean and separate runs and extras for better feature clarity.

## Project Components

### 1. Preprocessing
- Missing features like the bowling team and winning team were manually added.
- Regex was applied to split the `runs` column into numerical runs and extras, removing tags such as "W" and "NB".

### 2. Data Visualization
- Built an interactive web app using Dash for visualizing player and team statistics.
- Key functionalities include:
  - A slider to toggle between overs.
  - Dropdowns to select teams and players for comparison.
  - Dynamic graphs showcasing performance metrics such as runs scored, wickets taken, and match outcomes.

### 3. Predictive Modeling
- **Focus**: Predicting the performance of batsmen (runs scored) and bowlers (wickets taken).
- **Model**: A linear regression model was used due to its interpretability and simplicity.
- **Metrics**: The model was evaluated using Mean Squared Error (MSE).
- **Results**:
  - **Bowlers**: The model effectively predicts bowlers' wickets with an MSE of 1.17.
  - **Batsmen**: The model's run predictions for batsmen were less accurate, with an MSE of 53.45.
  - **Feature Importance**: The most important features affecting performance were the number of balls faced by batsmen and the number of balls bowled by bowlers.

### Usage
- The Dash web app allows you to visualize and compare player statistics.
- Use the slider to navigate through overs and the dropdowns to select teams or players.
- Analyze batting and bowling statistics, including average runs scored, strike rates, wickets taken, and runs conceded.
  
### Future Work
- Improve the accuracy of the linear regression model for predicting batsmen's runs.
- Expand the project to include additional predictive models and advanced statistical analysis.
  
## Project Report
[Click here to read more about the project](https://drive.google.com/file/d/1XbnGVR8BAg7dFhreJKAl4cB-hanW_DNx/view?usp=sharing)
