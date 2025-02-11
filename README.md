# IBM-DataScience-Projects
The projects that were completed during the IBM Data Science professional certificate course.
1. # DataScienceEcosystem Project
     This project was a test project for the course that showed the use of basic Python arithmetic.


2. # Tesla and GameStop Revenue Dashboard Project  (Graphs aren't visible for some reason)

      ## Overview  
      This project is part of an advanced data science curriculum to demonstrate the practical application of data extraction, analysis, and visualization techniques. As a data scientist working for an investment firm, you are tasked with creating an interactive dashboard to compare the stock prices of **Tesla** and **GameStop** against their revenue. This project integrates skills learned in previous labs, including **YFinance** for financial data retrieval and **web scraping** to obtain       
      revenue data.  
      
      ## Project Objectives  
      - **Data Extraction**: Use the YFinance library to gather historical stock price data for Tesla and GameStop.  
      - **Web Scraping**: Extract revenue data for both companies from relevant financial reports or websites.  
      - **Data Visualization**: Build a comprehensive dashboard to visualize and compare stock prices and revenue trends over time.  
      - **Peer Review**: Evaluate a peer's submission and provide constructive feedback, as part of the grading process.  
      
      ## Key Features  
      1. **Stock Price Analysis**:  
         - Retrieve and plot historical stock price data for Tesla and GameStop using the YFinance API.  
         - Ensure the data is cleaned and processed for accurate visualization.  
      
      2. **Revenue Data Extraction**:  
         - Implement web scraping techniques to gather revenue data from reliable financial websites.  
         - Clean and format the data for analysis and visualization.  
      
      3. **Dashboard Creation**:  
         - Build an interactive dashboard using tools such as Matplotlib, Plotly, or Dash.  
         - Compare trends in stock prices and revenue for Tesla and GameStop side by side.  
      
      4. **Submission and Peer Review**:  
         - Upload screenshots of your code and results to document your work.  
         - Review and grade a peer's submission as part of a collaborative learning experience.  
      
      ## Prerequisites  
      Before starting this project, ensure you have completed the following:  
      - **YFinance Lab**: Learn how to extract stock price data programmatically.  
      - **Web Scraping Lab**: Gain experience in extracting and processing data from web pages.  
      
      ## Deliverables  
      1. **Codebase**: A Python script that includes:  
         - Data extraction using YFinance.  
         - Revenue data scraping.  
         - Dashboard creation.  
      2. **Screenshots**: Upload screenshots of your working code and resulting visualizations.  
      3. **Dashboard**: A fully functional dashboard comparing Tesla and GameStop stock prices vs revenue.  
      4. **Peer Review**: Constructive feedback on one peer's project submission.  
      
      ## Tools and Libraries  
      - **YFinance**: To gather stock price data.  
      - **BeautifulSoup/Selenium**: For web scraping revenue data.  
      - **Matplotlib/Plotly/Dash**: For data visualization and dashboard development.  
      
      ## Learning Outcomes  
      - Apply financial data extraction and web scraping skills in a real-world context.  
      - Build an end-to-end data analysis and visualization solution.  
      - Enhance collaborative skills through peer review and feedback.  
      
      ## How to Run the Project  
      1. Clone the repository and navigate to the project directory.  
      2. Install the required dependencies listed in `requirements.txt`.  
      3. Run the Python script to extract data and generate visualizations.  
      4. Review the screenshots in the `screenshots` folder for the results.  
3. # Chicago Data Analysis Project

## Overview

This project aims to analyze a subset of Chicago's data, focusing on three primary datasets: **Census Data**, **Public Schools Data**, and **Crime Data**. The data is stored in an SQLite database, and various SQL queries are run to extract meaningful insights regarding crime patterns, education, and community economics in the city of Chicago.

The datasets used in this project are as follows:
- **Chicago Census Data**: Contains information about community areas in Chicago, including demographics, per capita income, and poverty statistics.
- **Chicago Public Schools Data**: Provides details about Chicago public schools, including their safety scores, types, and other related statistics.
- **Chicago Crime Data**: Records information about criminal activity across the city, including crime types, locations, and other attributes.

## File Structure

### `README.md`
- This file, explaining the purpose of the project and its structure.

### `FinalDB.db`
- The SQLite database where the datasets are loaded and analyzed.
  
### `notebooks/`
- A folder containing Jupyter notebooks or Python scripts used to load data, create tables, and execute SQL queries to analyze the data.

### `queries.sql`
- Contains SQL queries to analyze the data, such as retrieving crime information, community statistics, and school safety data.

## Data Sources

The datasets used in this project are available from the following URLs:

1. **Chicago Census Data**:  
   [Chicago Census Data CSV](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/FinalModule_Coursera_V5/data/ChicagoCensusData.csv)

2. **Chicago Public Schools Data**:  
   [Chicago Public Schools CSV](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/FinalModule_Coursera_V5/data/ChicagoPublicSchools.csv)

3. **Chicago Crime Data**:  
   [Chicago Crime Data CSV](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork/labs/FinalModule_Coursera_V5/data/ChicagoCrimeData.csv)

These datasets have been subsetted and pre-processed to match the format of the SQL queries for ease of use.

## Database Structure

The data is stored in an SQLite database, **FinalDB.db**, which contains the following tables:

1. **CENSUS_DATA**:  
   Contains community area data, including community area number, name, per capita income, and other demographic details.

2. **CHICAGO_PUBLIC_SCHOOLS**:  
   Contains information about public schools, including their safety score, type, and school name.

3. **CHICAGO_CRIME_DATA**:  
   Contains crime records, including case numbers, types of crime, and locations.

## SQL Queries and Analysis

This project involves executing various SQL queries to extract valuable insights from the data. Some example problems include:

1. **Problem 1**: Find the total number of crimes recorded in the crime dataset.
2. **Problem 2**: List all community area names and numbers with per capita income less than $11,000.
3. **Problem 3**: List all case numbers for crimes involving minors.
4. **Problem 4**: List all kidnapping crimes involving a child.
5. **Problem 5**: List the kinds of crimes recorded at schools.
6. **Problem 6**: List the type of schools along with the average safety score for each type.
7. **Problem 7**: List 5 community areas with the highest % of households below the poverty line.
8. **Problem 8**: Identify the most crime-prone community area.
9. **Problem 9**: Find the community area with the highest hardship index.
10. **Problem 10**: Determine the community area with the most number of crimes.

The queries are executed in the Python environment using the SQLite library, and the results are displayed using Pandas.

## Setup Instructions

1. **Install Required Libraries**  
   To run the project, make sure you have the following Python libraries installed:
   ```bash
   pip install pandas sqlite3 ipython-sql prettytable
   ```

2. **Database Setup**  
   The datasets will be loaded into the SQLite database **FinalDB.db** using the provided Python scripts. The scripts also include SQL queries to load the data into the database.

3. **Running Queries**  
   You can run the provided queries through Jupyter notebooks or any Python environment with SQLite support.

## Conclusion

This project demonstrates the use of SQL for data analysis by extracting insights from large datasets. By leveraging Pandas for data manipulation and SQLite for database management, the project provides an easy-to-use solution for analyzing complex data like crime, education, and census information. The queries cover a broad spectrum of analysis, from community economics to crime trends.

# 4. House Sales in King County

# Real Estate Housing Price Prediction

# House Sales in King County, USA

## Overview
This project analyzes house sales data in King County, USA, using a Jupyter Notebook. The dataset includes various features related to house pricing, such as square footage, number of bedrooms and bathrooms, location, and other attributes. The goal is to explore patterns, perform data preprocessing, and build predictive models for house prices.

## Project Structure
The project consists of the following key components:

- **`House_Sales_in_King_Count_USA.ipynb`**: A Jupyter Notebook that contains the entire data analysis workflow, including:
  - Data loading and preprocessing
  - Exploratory data analysis (EDA)
  - Feature engineering
  - Model building and evaluation
  - Insights and conclusions

- **Dataset**: The dataset used in this analysis consists of house sales records from King County, including Seattle. It contains information such as:
  - Sale price
  - Number of bedrooms and bathrooms
  - Square footage of living space and lot
  - Condition and grade of the house
  - Geographic location details (longitude and latitude)
  - Year built and year of renovation

## Methodology
The project follows a structured approach:

1. **Data Loading & Cleaning**
   - Importing the dataset
   - Handling missing values
   - Converting data types where necessary

2. **Exploratory Data Analysis (EDA)**
   - Statistical summaries
   - Visualizations (e.g., histograms, scatter plots, correlation heatmaps)
   - Identifying trends and patterns in house prices

3. **Feature Engineering**
   - Creating new features
   - Transforming existing features for better model performance

4. **Model Building & Evaluation**
   - Splitting data into training and testing sets
   - Training regression models (e.g., Linear Regression, Random Forest)
   - Evaluating model performance using RMSE, R², and other metrics

## Key Findings
- The price of a house is significantly influenced by factors such as square footage, location, and house condition.
- Waterfront properties tend to have a higher average price.
- Renovated houses and newer constructions generally sell for more.







