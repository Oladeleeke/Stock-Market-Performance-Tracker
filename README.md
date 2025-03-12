# Stock-Market-Performance-Tracker
I built a Stock Market Performance Tracker to analyze and compare the historical performance of Renewable Energy vs. Oil Stocks 
Introduction/Overview

I built a Stock Market Performance Tracker to analyze and compare the historical performance of Renewable Energy vs. Oil Stocks using SQL, Python (pandas, yfinance), and Azure Data Studio. The dataset includes price trends and trading volumes of major companies like:
Tesla (TSLA), 
ExxonMobil (XOM), 
BP, 
Chevron (CVX),
Enphase Energy (ENPH), 
NextEra Energy (NEE).

Key Steps & Technologies Used:
Data Extraction: Fetched stock data from Yahoo Finance using yfinance in Python
Data Cleaning & Transformation: Processed multiple stock attributes (Open, High, Low, Close, Volume) into a structured format.
Database Design: Created a relational database in SQL Server (Azure Data Studio) to store the stock data efficiently.
Data Loading: Used BULK INSERT to import large datasets into SQL tables.

Analysis & Insights:

Identified price growth trends over different time periods.
Compared volatility between Renewable Energy & Oil stocks.
Calculated average trading volumes to gauge investor activity.

Step 1, How i pulled the data set using python

#Install required libraries

<img width="356" alt="image" src="https://github.com/user-attachments/assets/079ab5a4-7787-4854-a713-f1b3e0bf027f" />


#import libraries

![image](https://github.com/user-attachments/assets/4d3f50ba-bca3-4108-bc9a-05a9dd29adc1)

# Define stock tickers. I selected Tesla (TSLA), ExxonMobil (XOM), BP (BP), Chevron (CVX), Enphase Energy (ENPH), and NextEra Energy (NEE) as our companies of interest.


![image](https://github.com/user-attachments/assets/d18a30c7-7fe9-4076-9009-138012c2a78e)

#Since the downloaded dataset has a MultiIndex format, we extracted specific columns separately.

#2.1 Extract and Save 'Close' Prices

 ![image](https://github.com/user-attachments/assets/255b7d7b-bae6-489d-bf76-99618a5002d2)

#Extract and Save 'Open' Prices

 ![image](https://github.com/user-attachments/assets/5c6cc75a-53fc-4fdc-a4b0-c693478aef74)


#Extract and Save 'Volume' Data

![image](https://github.com/user-attachments/assets/1aa7de26-2e25-4875-8d95-e1044b8ab693)


#Extract and Save 'Low' Prices

![image](https://github.com/user-attachments/assets/f7aac43e-bb26-4e02-962c-783337f64003)


#Extract and Save 'High' Prices

![image](https://github.com/user-attachments/assets/525a1e44-4cba-4599-9932-d57674cd1158)



#Save All Data into a CSV File
#Instead of separate CSV files, we combined them into one Excel file with multiple sheets for better organization.

![image](https://github.com/user-attachments/assets/db936fa8-92a7-4071-a29c-dbb23762c78e)


I uploaded the csv file onto msql and started to analyse and got familiar with my data, then i made the following analysis. 

--Stock performance Analysis
--What is the average closing price for each stock over the entire period?

![image](https://github.com/user-attachments/assets/46051c03-cffa-47b2-a32a-59e40a31a1dd)

![image](https://github.com/user-attachments/assets/e3b8925d-ec31-42ef-8f0b-0509272ffc3d)


--What is the highest and lowest price each stock has reached?

![image](https://github.com/user-attachments/assets/48551769-cb1b-4eef-b770-ce66d9ae0829)


![Screenshot 2025-03-12 at 1 17 05 PM](https://github.com/user-attachments/assets/a3c8f5e9-5693-4c08-9330-2c02f28e5e08)


--What was the daily percentage change for each stock?

![image](https://github.com/user-attachments/assets/973f25a5-ebff-4c14-8b04-ddb502ef5b16)


![image](https://github.com/user-attachments/assets/78df89fd-337d-4d9d-b802-63a5802a04a9)


--Which stock had the highest average trading volume?

![image](https://github.com/user-attachments/assets/a70105b6-21b0-4cd5-8c38-2671665720d3)

![image](https://github.com/user-attachments/assets/a487ea37-1273-459b-9af1-5cdf7101e831)


--Stock Trends & Market Comparisons
--What are the best-performing stocks over the last year?

![image](https://github.com/user-attachments/assets/266d4d62-c224-43d0-9455-df82275224e6)


![image](https://github.com/user-attachments/assets/52abc866-6899-4ffd-b6fb-e7d396567604)


--How do renewable energy stocks (e.g., Tesla, Enphase, NEE) compare to oil stocks (ExxonMobil, BP, Chevron)?


![image](https://github.com/user-attachments/assets/4ed3f337-aa35-4a6b-b348-b752b3f75196)


![image](https://github.com/user-attachments/assets/7cc17264-f63e-4a2e-9cda-d16e6e49f691)


--What was the best stock each year?

![image](https://github.com/user-attachments/assets/ca7ff528-d20e-40af-a033-31ae885abf4e)


![image](https://github.com/user-attachments/assets/8c4ea85f-e1b8-4e9d-82ec-be679b8eb682)


--What were the worst-performing stocks in a given time period?

![image](https://github.com/user-attachments/assets/a87c3e43-a421-4f78-b03f-3cb99b8390c8)


![image](https://github.com/user-attachments/assets/6ccfe6f7-94eb-4b8f-ae55-de574a39e78d)

Conclusion

This project provided valuable insights into the historical performance and volatility of Renewable Energy vs. Oil Stocks using SQL and data analysis techniques. By extracting, cleaning, and storing stock market data in a structured database, I was able to efficiently analyze key metrics such as price growth trends, volatility, and trading volume patterns.  

Through this process, I deepened my expertise in SQL, data modeling, and Python-based data automation, while also improving my ability to handle large datasets in Azure Data Studio. The findings from this analysis could help investors better understand market trends and make informed decisions.  

Going forward, I plan to enhance this project by integrating Looker Studio for interactive visualizations and expanding the dataset to include additional economic and financial indicators for deeper insights.  

This project has been a great learning experience, reinforcing my skills in data Analysis, database management, and financial analysis. 

