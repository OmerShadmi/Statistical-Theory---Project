# Statistical-Theory---Project
This is our final project in the course "Statistical Theory", by Ron Libman (211540265) and Omer Shadmi (327722575). 

## Project Overview

This project explores the hypothesis that left-footed footballers may have specific advantages in football skills compared to right-footed players. Using data from the FIFA19 dataset, which contains stats for over 18,000 players, we applied a variety of statistical techniques and machine learning models to assess differences between left-footed and right-footed players in attributes like crossing, dribbling, curve, and freekick accuracy.

### Key Attributes Analyzed:
- **Crossing**
- **Dribbling**
- **Curve**
- **Freekick Accuracy**

### Objectives
1. Analyze whether left-footed players outperform right-footed players in key attributes.
2. Use statistical tests to determine significant differences.
3. Apply machine learning models to understand the predictive importance of foot preference on player performance.

## Project Structure

This repository contains the following files:
- **`Statistical_Theory_Final_Project.ipynb`**: The Colab notebook containing all code for data processing, statistical analysis, visualizations, and machine learning models.
- **`Statistical_Theory_Final_Project.pdf`**: A comprehensive report summarizing the findings and methodologies used in the project.
- **`fifa_players.csv`**: The dataset containing statistics for 18,000 football players used in the analysis.
- **`requirements.txt`**: A list of required Python libraries to run the notebook.
- **`README.md`**: This file, which provides an overview of the project.


## Data Source

The dataset used for this project was taken from the FIFA19 dataset. It includes attributes for over 18,000 players, with various features such as:
- Preferred foot (left or right)
- Key performance attributes (e.g., dribbling, crossing, curve, freekick accuracy)
- Physical features (e.g., height, weight)
- Positional categories (e.g., forward, midfield, defense)
- Age, rating, and more.

## Analysis and Methodology

### 1. **Data Preprocessing**
   - We imported the FIFA19 dataset into the notebook using Pandas.
   - The data was cleaned to remove any missing values or irrelevant columns.
   - Players were divided into categories based on their **preferred foot**, **position**, **age**, **rating**, and other characteristics.
   
### 2. **Exploratory Data Analysis (EDA)**
   - Basic statistics and visualizations (such as histograms and radar plots) were generated to explore the distribution of player attributes between left-footed and right-footed players.

### 3. **Statistical Tests**
   To determine if there are significant differences between left-footed and right-footed players, we conducted several statistical tests:
   - **Welch's t-test**: Used to compare the means of two independent groups.
   - **Mann-Whitney U-test**: A non-parametric test to compare the distributions of two groups.
   - **Kolmogorov-Smirnov test**: Used to compare the cumulative distributions of the two groups.

### 4. **Machine Learning Models**
   - **XGBoost**: We trained an XGBoost model to predict key player attributes based on features such as foot preference, physical attributes, and technical skills.
   - **Feature Importance**: Using SHAP values and feature importance metrics, we assessed the predictive impact of foot preference on specific skills.

## Results

Our analysis found that left-footed players generally showed stronger performance in specific technical attributes, such as:
- **Crossing**
- **Dribbling**
- **Curve**
- **Freekick Accuracy**

However, the impact of foot preference on overall player effectiveness was limited, and the differences in skill ratings might be influenced by factors like the rarity of left-footedness and strategic deployment of players.

### Visualizations:
- **Radar Plot**: Visualizing the comparison of key attributes between left-footed and right-footed players.
- **Distribution Plot**: Showing the spread of dribbling skill ratings by foot preference.
- **Statistical Test Results**: Summarizing the outcomes of Welch’s t-test, Mann-Whitney U-test, and Kolmogorov-Smirnov test.

## Conclusion

While left-footed players demonstrated some advantages in specific skills, the overall impact of foot preference on performance is not unequivocally. The rarity of left-footed players and potential biases in player deployment may play a role in the observed differences.

## Limitations and Future Research

While this project included a robust analysis, there are some limitations:
- Although we accounted for position, age, height, and rating, more granular tactical data (e.g., playing time, team strategies) could provide deeper insights.
- The stats we've used were taken from the FIFA official game, although the stats are been written by professional football scouts and experts, they're still subjective, and are not brute fact. 
- Further studies could investigate the role of cognitive factors, such as the right hemisphere's involvement in creativity, which may offer an additional explanation for the advantage of left-footed players.

## Installation and Usage

To run the analysis locally, clone this repository and ensure you have the required Python packages installed. You can either run the notebook in Google Colab or set up the environment locally as follows:

### Required Libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `sklearn`
- `xgboost`
- `scipy`
- `shap`

### Running the Notebook

