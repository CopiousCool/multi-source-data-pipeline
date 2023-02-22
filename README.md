# multi-system-data-pipeline
A data pipeline that exposes and links data from multiple systems such as Looker and Lucidchart 

 Objective
 
Identify the data sources: The first step is to identify the different data sources that you want to pull data from. In this case, the sources are Looker and Lucidchart.

Extract the data: Once you have identified the data sources, the next step is to extract the data from each source. This can be done using APIs provided by the respective systems. For example, Looker provides a RESTful API that can be used to extract data from the Looker system.

Transform the data: After extracting the data, you may need to perform some transformations on it to ensure that it is in a format that can be used by your data pipeline. This might involve cleaning the data, reformatting it, or joining it with other data sources.

Load the data: Once the data has been extracted and transformed, the next step is to load it into a central repository or data warehouse. This could be a cloud-based solution such as Amazon Redshift, Google BigQuery, or Microsoft Azure SQL Data Warehouse.

Link the data: With the data now stored in a central repository, you can link it together using a data modeling tool. Looker provides a data modeling layer that allows you to build relationships between different tables of data.

Expose the data: Finally, you can expose the data to users via a BI tool such as Looker or Power BI. This allows users to create dashboards and reports that draw on data from multiple sources.

# Code Analysis / Documentation

This code defines three functions to read data from Looker and Lucidchart, and to merge the data from both sources. The read_looker_data() function takes a Looker API query as input, runs the query using the Looker API, and returns the results as a pandas dataframe. The read_lucidchart_data() function takes a file path as input, reads data from a CSV file using pandas.read_csv(), and returns the data as a pandas dataframe. The merge_data() function reads data from Looker and Lucidchart using the previously defined functions, merges the data using pandas.merge(), and returns the merged data as a pandas dataframe. Finally, the merge_data() function is called and the resulting merged data is printed to the console.
