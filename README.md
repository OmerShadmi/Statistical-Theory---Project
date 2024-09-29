# Statistical-Theory---Project
This is our final project in the course "Statistical Theory", by Ron Libman (211540265) and Omer Shadmi (327722575). 

### Table of Contents
1. [Project Overview](#project-overview)
   - [Key Attributes Analyzed](#key-attributes-analyzed)
   - [Objectives](#objectives)
2. [Project Structure](#project-structure)
3. [Data Source](#data-source)
4. [Analysis and Methodology](#analysis-and-methodology)
   - [1. Data Preprocessing](#1-data-preprocessing)
   - [2. Exploratory Data Analysis (EDA)](#2-exploratory-data-analysis-eda)
   - [3. Statistical Tests](#3-statistical-tests)
   - [4. Machine Learning Models](#4-machine-learning-models)
5. [Results](#results)
   - [Visualizations](#visualizations)
6. [Conclusion](#conclusion)
7. [Limitations and Future Research](#limitations-and-future-research)
8. [Installation and Usage](#installation-and-usage)
   - [Required Libraries](#required-libraries)
   - [Running the Notebook on Google Colab](#running-the-notebook-on-google-colab)
       - [1. Download the Necessary Files](#1-download-the-necessary-files)
       - [2. Open Google Colab](#2-open-google-colab)
       - [3. Upload the Notebook and Dataset](#3-upload-the-notebook-and-dataset)
       - [4. Install the Required Libraries](#4-install-the-required-libraries)
       - [5. Running the Notebook](#5-running-the-notebook)
       - [6. Saving Your Work](#6-saving-your-work)


## Project Overview

This project explores the hypothesis that left-footed footballers may have specific advantages in football skills compared to right-footed players. Using data from the FIFA19 dataset, which contains stats for ~18,000 players, we applied a variety of statistical techniques and machine learning models to assess differences between left-footed and right-footed players in attributes like crossing, dribbling, curve, and freekick accuracy.

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

### Visualizations:
- **Radar Plot**: Visualizing the comparison of key attributes between left-footed and right-footed players.
- **Distribution Plot**: Showing the spread of dribbling skill ratings by foot preference.
- **Statistical Test Results**: Summarizing the outcomes of Welch’s t-test, Mann-Whitney U-test, and Kolmogorov-Smirnov test.
- **SHAP Values**: Showing feature importance for specific player attributes.

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
- `statsmodels`

### Running the Notebook on Google Colab

To run the **`Statistical_Theory_Final_Project.ipynb`** notebook on Google Colab, follow these steps:

#### 1. Download the Necessary Files
First, download the following files from this repository:
- **`Statistical_Theory_Final_Project.ipynb`**: The Colab notebook.
- **`fifa_players.csv`**: The dataset used in the analysis.
- **`requirements.txt`**: The text file containing the required libraries.

#### 2. Open Google Colab
Navigate to [Google Colab](https://colab.research.google.com/).

#### 3. Upload the Notebook and Dataset
- Click on **"File"** → **"Upload notebook"** and upload the **`Statistical_Theory_Final_Project.ipynb`** file.
- Then, upload the **`fifa_players.csv`** dataset and **`requirements.txt`** file by clicking on the **"Files"** icon on the left pane and selecting **"Upload to session storage"**.

#### 4. Install the Required Libraries
Once the notebook is open, ensure that all required libraries are installed. Run the following command in a code cell to install the dependencies:

!pip install -r requirements.txt

#### 5. Running the Notebook
Once the libraries are installed, you can run each cell in the notebook by clicking "Runtime" → "Run all" or by running cells individually.

The notebook contains code for data processing, statistical analysis, and visualizations. Make sure all the cells execute successfully to view the full analysis and outputs.

#### 6. Saving Your Work
To save the notebook with your outputs, you can download it by clicking "File" → "Download" and choosing the format you'd like (e.g., .ipynb).

By following these steps, you can run the analysis and explore the insights into the performance differences between left-footed and right-footed football players.
