Loading Online Event Hits using SQOOP to HIVE via Shell Script
![scd](https://user-images.githubusercontent.com/107995859/193507903-1e8be2d0-c1bc-44d8-b498-b8ccb8e941f2.jpeg)


Creating a script to automate data load in HDFS with reconciliation of data

1- At first I have written a script to automate reading of new files from archive folder and transferred data in MySQL.

2- Created a Sqoop Job which will use Sqoop Incremental Operation to send data in HDFS (Hadoop File System).

3- Created Managed Table in Hive and then transferred data from HDFS to hive table.

4- Then Created External table with dynamic partition on bases of (year, month) and load data into external table from managed table with SCD1 Logic.

5- At last exported updated data from hive table to SQL for data reconciliation
