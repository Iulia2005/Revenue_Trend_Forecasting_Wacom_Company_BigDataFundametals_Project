# Project Title:Sales Forecasting — Video Game Global Sales 

========== 1. Project Description ========== 
This project analyzes worldwide video game sales data between 1980 to 2020, covering 16,598 games across 31 platforms and 12 genres. The goal is to identify sales trends by genre, platform, and region, and to build a predictive model that estimates a game's global sales based on its characteristics and regional performance.

========== 2. Dataset ========== 
Source: The dataset was found on kaggle.com (https://www.kaggle.com/datasets/willianoliveiragibin/video-game-sales-analyze)
Description: The dataset includes 11 columns (Rank, Name, Platform, Year, Genre, Publisher, NA_Sales, EU_Sales, JP_Sales, Other_Sales, Global_Sales) covering video game sales worldwide from 1980 to 2020.

========== 3. Technology Stack ========== 
Language: Python 3.12.9
Data Processing: Pandas, PySpark 3.5.3
Visualization: Power BI
Version Control: GitHub

========== 4. Pipeline Architecture ========== 
1. Data Ingestion: Dataset downloaded from Kaggle as a CSV file
2. Preprocessing: Handled 271 missing Year values (median imputation), 58 missing Publisher values (filled with "Unknown"), removed duplicates, detected outliers using IQR method, and engineered new features (Sales_Gap, JP_Share, Genre_Encoded, Platform_Encoded)
3. Analysis: EDA revealed Action as the top selling genre and PS2 as the top selling platform. Sales peaked globally around 2008-2009. A Random Forest Regressor was trained to predict Global_Sales using regional sales and game characteristics as features.
4. Output: Power BI dashboard with 4 visuals — Sales by Genre, Sales by Platform, Sales Trend Over Time, and Top 10 Best Selling Games.

========== 5. Installation & Usage ========== 
1. Clone the repository: https://github.com/Iulia2005/Sales_Forecating_BigDataFundametals_Project.git
2. Install dependencies: pip install pandas matplotlib seaborn scikit-learn pyspark jupyter
3. Run the main notebook/script: jupyter notebook BigData_Project.ipynb

========== 6. Key Insights ========== 
Insight 1: Action is the best selling genre with over 1,500 million units sold globally, followed by Sports and Shooter.
Insight 2: Video game sales peaked around 2008-2009 and have been declining since, likely due to the rise of mobile and digital gaming.
Insight 3: PS2 is the top selling platform of all time in this dataset, followed by X360 and PS3.
Insight 4: NA_Sales is the strongest predictor of Global_Sales according to the Random Forest feature importance analysis.

========== 7. Author ========== 
Name: Serban Iulia Maria
Course: Big Data Fundamentals
