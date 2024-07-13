# BigData-Ops-on-TLC-Yellow-Taxi
Conducted big data analytics on New York City's Yellow taxi data set of the year 2017 (5.17 GB) with Big Data tools such as Hadoop, HBase, Sqoop, MapReduce, AWS EMR, AWS RDS (MySQL)

The data set for the assignment can be downloaded from these links:
https://nyc-tlc-upgrad.s3.amazonaws.com/yellow_tripdata_2017-01.csv
https://nyc-tlc-upgrad.s3.amazonaws.com/yellow_tripdata_2017-02.csv
https://nyc-tlc-upgrad.s3.amazonaws.com/yellow_tripdata_2017-04.csv
https://nyc-tlc-upgrad.s3.amazonaws.com/yellow_tripdata_2017-05.csv
https://nyc-tlc-upgrad.s3.amazonaws.com/yellow_tripdata_2017-06.csv

https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf

# Task

The Big Data tools used are the Hadoop Framework, Apache HBase, and Apache Sqoop. Utilize an AWS EMR instance with an m4.xlarge cluster (64 GB) that includes all necessary services, and install additional services as required (such as AWS RDS MySQL).

## Data Ingestion Tasks:

Task 1: Create an RDS instance in your AWS account and upload data from two files (yellow_tripdata_2017-01.csv & yellow_tripdata_2017-02.csv) from the dataset. Ensure that you create an appropriate schema for the datasets before uploading them to the RDS.

Task 2: Use the Sqoop command to transfer data from the RDS to the HBase Table.

Task 3: Perform a bulk import of data from the next two files in the dataset to your HBase Table on your EMR cluster using the relevant code. Note: For this task, only import data from the subsequent two CSV files.

## MapReduce Tasks:

Task 4: Write MapReduce codes to execute the following tasks using the files downloaded on your EMR Instance:

Identify which vendors have the most trips and determine the total revenue generated by each vendor.
Determine which pickup location generates the most revenue.
Identify the different payment types used by customers and their count, presenting the results in a sorted format.
Calculate the average trip time for various pickup locations.
Compute the average tips to revenue ratio for drivers at different pickup locations and present it in a sorted format.
Analyze how revenue varies over time by calculating the average trip revenue per month, broken down by hour of the day (day vs. night) and day of the week (weekday vs. weekend). Note: It's recommended to use MRJob for these MapReduce tasks.


