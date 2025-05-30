📊 Numerical Analysis of Stocks and Sales Data with NumPy
Date: 16/11/2024
Project Summary:
This project demonstrates how to use NumPy for analyzing stocks and sales data, focusing on various financial metrics across different market sectors. The analysis covers data cleaning, correlation calculations, sector-based analysis, outlier detection, and price trend evaluations — all performed using core NumPy functions without relying on additional libraries.

📁 Project Overview
The project involves:

Loading and preparing CSV data as NumPy structured arrays

Handling missing values and text data

Performing descriptive statistics and correlations

Detecting outliers and identifying market trends

Sector-based financial insights

📌 Tasks & Methods
1️⃣ Data Loading and Preparation
Task: Load CSV data into a NumPy structured array.

Explanation: Uses np.genfromtxt() to read the CSV, handling missing values as NaNs and ensuring the array is structured according to dataset column types.

Key Functions: np.genfromtxt()

2️⃣ Data Cleaning: Handle Missing and Text Values
Task: Identify and replace missing numeric values with the column mean.

Explanation: Detect missing values via np.isnan() and replace them using np.nanmean() to prepare data for analysis.

Key Functions: np.isnan(), np.nanmean()

3️⃣ Descriptive Statistics for Stock Prices by Sector
Task: Calculate mean, standard deviation, min, and max for opening and closing prices by sector.

Explanation: Summarizes price distributions and spreads across sectors.

Key Functions: np.mean(), np.std(), np.min(), np.max()

4️⃣ Price Comparison by Sector
Task: Compute average opening and closing prices per sector.

Explanation: Groups data by sector and applies np.mean() to highlight sectoral price variations.

Key Functions: np.mean()

5️⃣ Correlation Analysis of Opening and Closing Prices
Task: Calculate Pearson correlation between opening and closing prices.

Explanation: Uses np.corrcoef() to check if opening and closing prices are linearly related.

Key Functions: np.corrcoef()

6️⃣ Sector Analysis of Market Capitalization
Task: Group stocks by sector and calculate average market capitalization.

Explanation: Identifies unique sectors via np.unique() and computes mean capitalizations.

Key Functions: np.unique(), np.mean()

7️⃣ Identifying Highest and Lowest Stock Prices
Task: Find stocks with the highest and lowest opening and closing prices.

Explanation: Uses np.argmax() and np.argmin() to locate and retrieve these records.

Key Functions: np.argmax(), np.argmin()

8️⃣ Outlier Detection in Stock Prices
Task: Detect outliers using the Interquartile Range (IQR) method.

Explanation: Calculates Q1 and Q3 with np.percentile(), then identifies values outside 1.5×IQR.

Key Functions: np.percentile()

9️⃣ Comparing Stock Prices Against a Threshold
Task: Calculate the proportion of stocks with closing prices above a given threshold (e.g., $200).

Explanation: Uses logical operations and np.sum() to count and compute the percentage.

Key Functions: Logical operations, np.sum()

🔟 Trend Over Time (If Period Data Exists)
Task: Measure stock price changes over time for each stock.

Explanation: Applies np.diff() to track changes between consecutive time points.

Key Functions: np.diff()

📦 Requirements
Python 3.x

NumPy

📚 Conclusion
This project showcases NumPy's versatility in handling real-world financial data, offering efficient and insightful analysis tools for stock market trends, sector performance, and price behavior — all within a clean, dependency-free environment.
