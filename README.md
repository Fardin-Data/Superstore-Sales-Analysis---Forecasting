# Superstore Sales Analysis and Forecasting
<img src="https://github.com/Fardin-Data/Superstore-Sales-Analysis-and-Forecasting/assets/137788371/0d26d4a0-80cd-4f6e-bcb6-37af346c1fcc" width="1400">

# Table of Contents
- [Introduction](#introduction)
- [Process](#Process)
- [Dashboard](#Dashboard)
- [Sales Forecasting](#Sales-Forecasting)
- [Key Insights](#Key-Insights)
- [Tech Stack](#Tech-Stack)
- [Data Set](#Data-Set)
  
## Introduction

The Superstore Sales Insights & Forecasting aims to help users gain valuable insights from sales data and facilitate informed decision-making. The project comprises two main components:

# Process

`Data Preparation`
- Initially, I performed data cleaning tasks such as removing null values, eliminating unnecessary columns, handling duplicates, and adjusting data types to ensure data quality.

`Data Modeling`
- I proceeded to create calculated measures and tables using DAX (Data Analysis Expressions) in Power BI, enhancing the dataset's analytical capabilities.
<pre><code>
  #Making time series table
  SUMMARIZE(SuperStore_Sales_Dataset,SuperStore_Sales_Dataset[Order Date], "Total Sales", SUM(SuperStore_Sales_Dataset[Sales]))

  #Days it takes to deliver the order
  DATEDIFF(SuperStore_Sales_Dataset[Order Date],SuperStore_Sales_Dataset[Ship Date],DAY)
</code></pre>

`Data Analysis`
- Next, I conducted an in-depth data analysis within Power BI. I used various visualization techniques like matrices to identify trends in sales, region-wise sales, category-wise sales, and other relevant insights.

`Dashboard Creation`
- I then developed an interactive and dynamic dashboard using Power BI. This dashboard included bookmark features that facilitated seamless navigation between different charts and visualizations for a more comprehensive view of the data.

`Sales Forecasting`
- To provide forward-looking insights, I leveraged Power BI's advanced forecasting feature to perform a 10-day sales forecast, helping stakeholders anticipate future trends and make informed decisions.

## Dashboard

The dashboard section offers an array of visualizations that empower users to explore and understand historical sales data. Key features of the dashboard include:

- Visualization of monthly and yearly sales trends.
- Comparison of sales across different categories and sub-categories.
- Geographical distribution of sales.
- Identification of top payment modes, segments, ship modes, and much more.

![image](https://github.com/Fardin-Data/Superstore-Sales-Analysis-and-Forecasting/assets/137788371/6386d2e3-6773-4489-ab50-0ac8112416e5)

## Sales Forecasting

![Forecasting Report](https://github.com/Fardin-Data/Superstore_Sales_Insights_and_Forecasting/assets/137788371/e6350e18-85e5-4961-9e61-f8b0243f679d)


The sales forecasting page focuses on predicting sales for the subsequent 10 days. Leveraging historical sales data and advanced forecasting techniques, this predictive model enables users to interact with forecasted results.

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

- **Power BI Desktop**: Design, visualization, and interactive reporting.
- **DAX (Data Analysis Expressions)**: Creation of calculations and measures supporting data visualizations.
- **Advanced Analytics**: Predict future sales trends based on historical data.
- **Power Query**: Clean and transform raw data into a structured format.

## Data Set

The Superstore Sales Data used in this project can be accessed [here](https://drive.google.com/drive/folders/1t_r26xUjm5ZyEFFOF3AD1BmOvUgQaxd1?usp=sharing).

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute the code and visuals as long as the original license terms are maintained.

---

Enjoy exploring the Power BI Sales Insights and Forecasting Dashboard! If you have questions or feedback, feel free to contact me.

*Contact: fardinkhan.data@gmail.com*
