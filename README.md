FIFA World Cup Squads - Exploratory Data Analysis
📊 Project Overview
This project performs an Exploratory Data Analysis (EDA) on FIFA World Cup squads data using Python and Pandas. The analysis focuses on data cleaning, preprocessing, and extracting insights from player statistics across multiple World Cup tournaments (2014, 2018, 2022).

📁 Dataset
The dataset (fifa_world_cup_squads.csv) contains information about players who participated in the FIFA World Cup, including:

Player demographics (name, age, country, height)

Performance metrics (matches played, goals, assists, minutes played)

Club information and market value

Captaincy status and tournament year

Last updated timestamp

🔧 Key Analysis Performed
1. Data Loading & Inspection
Loaded dataset into pandas DataFrame

Displayed basic structure, statistical summaries, and data types

Identified numeric and text columns

2. Data Selection & Filtering
Used .loc[] and .iloc[] for data subsetting

Applied boolean masking for complex filters

Created subsets (e.g., players with 6+ matches, 2022 World Cup players)

3. Data Cleaning & Preprocessing
Missing Values: Identified and handled missing values in various columns

Disguised Missing Values: Replaced placeholders ('N/A', '-', '?', 'Unknown') with proper NaN

Data Type Conversion:

Converted Goals column from text to numeric

Cleaned Market Value (removed '€' and 'M' symbols)

Converted Last Updated to datetime format

Prepared Age for integer conversion

Duplicate Records: Detected and removed duplicates (both full row and by Player_ID)

Impossible Values: Identified and fixed impossible ages (0, >80) and negative goals

4. Missing Data Strategy
Numeric columns: Filled with mean or median based on distribution

Text columns: Filled with mode for categorical data

Justified each decision based on data characteristics

5. Exploratory Insights
Analyzed player distribution across World Cup years

Identified top goal scorer

Compared average goals between 2018 and 2022 tournaments

Analyzed market value differences between age groups

Observed inconsistencies in country naming conventions

📈 Key Findings
Top Scorer: Kim Min-jae (South Korea) with 9 goals in 2014

Goal Scoring Trend: 2018 had slightly higher average goals (2.25) compared to 2022 (2.12)

Market Value Insight: Younger players (≤30) have higher average market value (€67.9M) than older players (>30) (€64.8M)

Data Quality Issues: Country column has significant inconsistencies in spelling and casing

Missing Data: 41 missing age values, 23 missing matches_played, and disguised missing values in Goals and Market Value columns

🛠️ Technologies Used
Python 3.x

Pandas

NumPy

Google Colab (for notebook execution)

📝 How to Run
Clone this repository

Open the Jupyter notebook in Google Colab or Jupyter environment

Upload the fifa_world_cup_squads.csv file when prompted

Run all cells sequentially

📊 Sample Outputs
Data shape: 436 rows × 15 columns

Duplicates removed: 6 rows

Successfully converted all numeric columns to proper data types

Handled 52+ missing values in Market Value column

🔍 Future Work
Standardize country names and casing

Perform deeper analysis on positional trends

Create visualizations for better insights

Build predictive models for player performance

👩‍💻 Author
Rida - Data Science Assignment

📅 Date
2026-07-04

📚 Dependencies
python
import pandas as pd
import numpy as np
from google.colab import files
This project was completed as part of a data science assignment focusing on EDA and data cleaning techniques.

