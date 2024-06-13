# LOK-SABHA-CANDIDATES-
**Project Overview**

This project focuses on the extraction, transformation, and analysis of candidate data from the 2019 Lok Sabha elections in India. The objective is to create a comprehensive SQLite database from web-scraped data and perform various analytical and visualization tasks to gain insights into the political landscape, specifically regarding candidates' criminal cases, education, total assets, and liabilities.

**Data Extraction and Transformation**

Web Scraping: The data was scraped from the myneta.info website, which provides detailed information about candidates in Indian elections. Two URLs were used: one for candidates' criminal records and another for their educational qualifications.

Regular Expressions: To parse the HTML content, regular expressions were employed to extract relevant data from the tables on the web pages.

SQLite Database: The extracted data was stored in two separate SQLite tables:

criminal_cases: Contains data on candidates' criminal cases, education, total assets, and liabilities.
graduate_candidates: Contains data on candidates' educational qualifications.

**Data Merging and Cleaning**

Table Creation: A new table, Grad_Lok_Can, was created by joining the criminal_cases and graduate_candidates tables based on the candidates' names.

Data Cleaning: Missing values and inconsistencies were handled, such as converting asset and liability data to numerical types and ensuring all criminal cases were recorded as numerical values.

Descriptive Analysis
DataFrame Conversion: The combined data was converted into a Pandas DataFrame for ease of analysis.

Statistical Summary: The DataFrame was analyzed to provide a summary of the distribution of criminal cases, total assets, and liabilities.

**Visualization**

Pie Chart: Visualized the distribution of candidates' education levels in the Lok Sabha.

Histogram: Showed the distribution of criminal cases among candidates.

Scatter Plot: Illustrated the relationship between political parties and their candidates' criminal cases.

Bar Graph: Highlighted the top 10 political parties with the highest number of criminal cases.

**Predictive Analysis**

Linear Regression: A linear regression analysis was performed to understand the relationship between candidates' total assets and liabilities.

Decision Tree Regression: A decision tree regressor was used to explore the relationship between candidates' total assets and the number of criminal cases.

**Text Analysis**

Frequency Analysis: Conducted frequency analysis on the Party and Education columns to identify the most common values.

**Conclusion**

This project provided a detailed examination of the candidates' profiles in the 2019 Lok Sabha elections. It showcased the use of web scraping, data cleaning, database management, descriptive statistics, data visualization, and predictive modeling to draw meaningful insights from complex datasets. The findings offer a nuanced view of the intersection between candidates' criminal backgrounds, education, and financial standing, contributing to a better understanding of electoral dynamics in India. This comprehensive analysis can be found in my GitHub portfolio, demonstrating my skills in data science, including data extraction, transformation, and visualization, as well as predictive analytics.
