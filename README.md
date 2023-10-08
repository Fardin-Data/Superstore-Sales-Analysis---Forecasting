# Superstore Sales Analysis and Forecasting
<img src="https://github.com/Fardin-Data/Superstore-Sales-Analysis-and-Forecasting/assets/137788371/0d26d4a0-80cd-4f6e-bcb6-37af346c1fcc" width="1400">

  
## Introduction
In today's business landscape, data-driven decision-making is crucial for success. The Superstore Sales Analysis and Forecasting project leverages the power of data to uncover patterns, trends, and key insights within a sales dataset. By employing advanced analytics and visualization techniques, this project assists stakeholders in understanding historical sales performance and predicting future trends.


## Process
`Data Preparation`
- The initial phase involved performing data cleaning tasks, including the removal of null values, the elimination of unnecessary columns, handling duplicates, and adjusting data types to ensure data quality.

`Data Modeling`
- The subsequent step was to create calculated measures and tables using DAX (Data Analysis Expressions) in Power BI, enhancing the dataset's analytical capabilities.
  
<pre><code>
  # Created time-series table of sales for forecasting.
  TimeSeriesTable = 
  SUMMARIZE(
    SuperStore_Sales_Dataset,
    SuperStore_Sales_Dataset[Order Date],
    "Total Sales", SUM(SuperStore_Sales_Dataset[Sales])
  )  
  
  # Calculate a measure to determine the number of days it took for delivery.
  DaysToDeliver = 
  DATEDIFF(
    SuperStore_Sales_Dataset[Order Date],
    SuperStore_Sales_Dataset[Ship Date],
    DAY
  )
</code></pre>

`Data Analysis`
- Following data modeling, an in-depth data analysis was conducted within Power BI, utilizing various visualization techniques like matrices to identify trends in sales, region-wise sales, category-wise sales, and other pertinent insights.

`Dashboard Creation`
- The project proceeded with the development of an interactive and dynamic dashboard in Power BI. This dashboard was designed to include bookmark features, allowing for seamless navigation between different charts and visualizations to provide a more comprehensive view of the data.

`Sales Forecasting`
- To deliver forward-looking insights, Power BI's advanced forecasting feature was utilized to perform a 10-day sales forecast. This forecasting capability assists stakeholders in anticipating future trends and making informed decisions.
## Dashboard
The dashboard section offers an array of visualizations that empower users to explore and understand historical sales data. Key features of the dashboard include:

- Visualization of monthly and yearly sales trends.
- Comparison of sales across different categories and sub-categories.
- Geographical distribution of sales.
- Identification of top payment modes, segments, ship modes, and much more.

![image](https://github.com/Fardin-Data/Superstore-Sales-Analysis-and-Forecasting/assets/137788371/6386d2e3-6773-4489-ab50-0ac8112416e5)

## Sales Forecasting

![Forecasting Report](https://github.com/Fardin-Data/Superstore_Sales_Insights_and_Forecasting/assets/137788371/e6350e18-85e5-4961-9e61-f8b0243f679d)

The sales forecasting page focuses on predicting sales for the subsequent 10 days. Leveraging historical sales data and advanced forecasting techniques of Power BI.

## Key Insights
The dashboard and forecasting page unveil the following key insights:

1. **Monthly Peaks**: Noteworthy sales spikes in February, August, and October hint at recurring patterns.
2. **Parallel Growth**: While 2020 exhibits higher sales than 2019, the trend patterns remain consistent.
3. **Geographic Leaders**: California takes the lead in sales, closely followed by New York.
4. **Region Impact**: The West region contributes the most to overall sales.
5. **Payment Preference**: Cash On Delivery (COD) emerges as the preferred payment method.
6. **Consumer Champion**: The consumer segment generates the highest sales figures.
7. **Top Category**: Office Supplies stand out as the dominant sales category.
8. **Preferred Shipping**: Standard Class is the preferred shipping choice.
9. **Sub-Category Stars**: Phones and chairs emerge as the top-selling sub-categories.

## Tech Stack
Project relies on the following key technologies:

- `Power BI Desktop` Design, visualization, and interactive reporting.
- `DAX (Data Analysis Expressions)` Creation of calculations and measures supporting data visualizations.
- `Advanced Analytics` Predict future sales trends based on historical data.
- `Power Query` Clean and transform raw data into a structured format.

## Files Information
`Data`

- **SuperStore Processed Data:** This file holds the data that has undergone cleaning and processing.
- **Sales TimeSeries:** This file includes an additional table created using DAX, which played a role in the forecasting process.

`Results`

- **Dashboard:** Within this section, you will find two sheets - one dedicated to the interactive dashboard and the other to the forecasting report.

## Data Source
The Superstore Sales Data used in this project can be accessed [here](https://drive.google.com/drive/folders/1t_r26xUjm5ZyEFFOF3AD1BmOvUgQaxd1?usp=sharing).

## License
This project is licensed under the MIT License. You are free to use, modify, and distribute the code and visuals as long as the original license terms are maintained.

---

Enjoy exploring the Power BI Sales Insights and Forecasting Dashboard! If you have questions or feedback, feel free to contact me.

*Contact: fardinkhan.data@gmail.com*
