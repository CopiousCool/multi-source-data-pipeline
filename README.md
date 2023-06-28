# multi-system-data-pipeline
A data pipeline that exposes and links data from multiple systems such as Looker and Lucidchart 

 Objective
 
Identify the data sources: The first step is to identify the different data sources that you want to pull data from. In this case, the sources are SalesForce, Looker and Lucidchart.

Extract the data: Once you have identified the data sources, the next step is to extract the data from each source. This can be done using APIs provided by the respective systems. For example, Looker provides a RESTful API that can be used to extract data from the Looker system.

Transform the data: After extracting the data, you may need to perform some transformations on it to ensure that it is in a format that can be used by your data pipeline. This might involve cleaning the data, reformatting it, or joining it with other data sources.

Load the data: Once the data has been extracted and transformed, the next step is to load it into a central repository or data warehouse. This could be a cloud-based solution such as Amazon Redshift, Google BigQuery, or Microsoft Azure SQL Data Warehouse or even a more modern Graph or Vector DB.

Link the data: With the data now stored in a central repository, you can link it together using a data modeling tool. Looker provides a data modeling layer that allows you to build relationships between different tables of data.

Expose the data: Finally, you can expose the data to users via a BI tool such as Looker or Power BI. This allows users to create dashboards and reports that draw on data from multiple sources.

# Code Analysis / Documentation

This code is a Python script that does the following:

It imports several Python packages that provide functionality for working with data, including pandas, the Salesforce API, and Lucidchart.
It defines three functions that are used to read data from different sources: Looker, Lucidchart, and Salesforce. The Looker and Lucidchart functions read data from CSV files, while the Salesforce function uses the Salesforce API to query data from Salesforce.
It defines a fourth function that uses the previously defined functions to merge data from all three sources into a single pandas dataframe.
Finally, the script calls the merge_data function and outputs the resulting merged data to the console.

The Python program is designed to read data from multiple sources, including Salesforce, Looker, and Lucidchart, and merge the data into a single dataframe. The program achieves this by defining several functions that use different methods to read data from each source.

For example, the read_salesforce_data() function uses the Salesforce API to query data from Salesforce, while the read_looker_data() and read_lucidchart_data() functions read data from CSV files. The program then uses the merge_data() function to combine the data from all three sources into a single dataframe using the pandas merge() function.

The program is flexible and can be customized to read data from different sources and combine them in different ways. For example, if you wanted to add a new data source, such as Google Sheets, you could create a new function to read data from Google Sheets and modify the merge_data() function to include the new data source.

Overall, this program provides a way to easily access and combine data from multiple sources, including Salesforce, Looker & Lucidchart, and performing data analysis using Python and pandas in one complete tool.

# Note

Note that you will need to replace the placeholder values 
'your_salesforce_username', 
'your_salesforce_password', 
'your_salesforce_security_token', 
'your_look_id', 
'your_look_view', 
'your_look_query', '
your_lucid_file_path', 
and 
'your_salesforce_query' 

with the appropriate values for your specific data sources and queries.
