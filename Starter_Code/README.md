# athletic_sales_analysis


## **Background** 
In this project, you'll analyze sales data to gain insights into various aspects of athletic wear sales over two years.
The analysis will focus on:

1. **Identifying which cities in the U.S. have sold the most athletic wear.**
2. **Determining which retailers had the greatest total sales for athletic wear.**
3. **Finding out which retailers sold the most women's athletic footwear.**
4. **Analyzing which day and week had the highest sales for women's athletic footwear.**

## **Instructions** ##

1. Combine and Clean the Data by using two CSV files, athletic_sales_2020.csv and athletic_sales_2021.csv, into DataFrames.
2. Verify that the columns in both DataFrames have similar names and data types.
3. Combine the two DataFrames by rows using an inner join.
4. Reset the index of the combined DataFrame.
5. Clean data:
    - Check for any null values.
    - Verify each column’s data type.
    - Convert the "invoice_date" column to a datetime data type.
    - Confirm that the conversion was successful.

6. Determine Which Region Sold the Most Products
   Using Multi-Index DataFrame:

    - Use groupby or pivot_table to aggregate data by "region", "state", and "city".
    - Rename Aggregated Column:

    - Rename the aggregated column to reflect the total number of products sold.
    - Sort the results in descending order to identify the top five regions with the greatest number of products sold.

7. Determine Which Region Had the Most Sales
    - Using Multi-Index DataFrame.
    - Use groupby or pivot_table to aggregate data by "region", "state", and "city".
    - Rename the aggregated column to reflect total sales.
    - Sort the results in descending order to find the top five regions with the highest sales.

4. Determine Which Retailer Had the Most Sales
    - Create a Multi-Index DataFrame.
    - Use groupby or pivot_table to aggregate data by "retailer", "region", "state", and "city".
    - Rename the aggregated column to reflect total sales.
    - Sort the results in descending order to find the top five retailers with the highest total sales.
5. Determine Which Retailer Sold the Most Women's Athletic Footwear
    - Filter Data:
    - Filter the combined DataFrame to create a subset with only women’s athletic footwear sales.
    - Create a Multi-Index DataFrame.
    - Use groupby or pivot_table to aggregate data by "retailer", "region", "state", and "city".
    - Rename the aggregated column to reflect the number of women’s athletic footwear units sold.
    - Sort the results in descending order to find the top five retailers with the highest sales of women’s athletic footwear.

6. Determine the Day with the Most Women's Athletic Footwear Sales
    - Create a pivot table with "invoice_date" as the index and "total_sales" as the values.
    - Apply resampling to daily bins to get total sales for each day.
    - Sort the resampled DataFrame in descending order to identify the top 10 days with the highest sales of women’s athletic footwear.
7. Determine the Week with the Most Women's Athletic Footwear Sales
    - Apply resampling to weekly bins to get total sales for each week.
    - Sort the resampled DataFrame in descending order to identify the top 10 weeks with the highest sales of women’s athletic footwear.

