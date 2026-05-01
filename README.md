# E-commerce-Sales-Analysis-using-Apache-Hive-in-Hadoop-Environment
1. Introduction
In the contemporary digital era, Big Data plays a pivotal role in the operational and strategic decision-making processes of modern businesses. E-commerce platforms generate massive volumes of structured, semi-structured, and unstructured data daily, encompassing user transactions, product catalog interactions, and geographical sales metrics. Traditional relational database management systems (RDBMS) often struggle to process these vast datasets efficiently.
To address these challenges, the Hadoop ecosystem provides a robust, distributed computing framework. At its core, the Hadoop Distributed File System (HDFS) enables the fault-tolerant storage of massive datasets across clusters of commodity hardware. Built on top of Hadoop, Apache Hive acts as a data warehouse infrastructure that facilitates reading, writing, and managing large datasets residing in distributed storage using SQL. Hive projects structure onto this data and allows users to query it using a SQL-like language called HiveQL (HQL). This abstraction eliminates the need to write complex Java MapReduce programs, making large-scale e-commerce data analysis accessible, efficient, and highly scalable.
2. Objectives
The primary objectives of this analytical project are as follows:
●	To store and process large-scale sales data securely and efficiently utilizing the Hadoop Distributed File System (HDFS).
●	To perform complex data analysis using Apache Hive by executing MapReduce jobs via high-level HiveQL queries.
●	To derive meaningful business insights from raw e-commerce sales data, including revenue generation patterns, category performance, and geographic sales distribution.
3. Tools and Technologies Used
●	Hadoop (HDFS): The underlying storage layer utilized to store the raw e-commerce data file. It provides high throughput access to application data and is suitable for applications with large datasets.
●	Apache Hive: The data warehousing component used to map the raw text data into a structured table format and query it using SQL-like syntax. Hive internally translates these queries into MapReduce jobs.
●	Cloudera Quickstart VM: A single-node Hadoop cluster deployment running on a virtual machine. It provides a comprehensive, pre-configured environment containing all essential Hadoop ecosystem components (HDFS, YARN, Hive, etc.) for development and testing.
●	Linux Terminal (Bash): The command-line interface used to interact with the local file system, execute HDFS shell commands, and launch the Hive CLI interface.
4. Dataset Description
The dataset used for this analysis represents daily transaction records of an e-commerce platform. It is stored locally as a comma-separated text file named sales.txt.
The structured schema maps to the following six columns:
1.	order_id (INT): A unique identifier for each transaction.
2.	product (STRING): The name of the item purchased.
3.	category (STRING): The overarching retail category of the product.
4.	price (INT): The unit price of the product.
5.	quantity (INT): The number of units purchased in the transaction.
6.	city (STRING): The geographical location where the order was placed.
Sample Dataset Entries:
1,Mobile,Electronics,15000,2,Delhi
2,Laptop,Electronics,55000,1,Mumbai
3,Shoes,Fashion,2000,3,Delhi
4,Tshirt,Fashion,800,5,Pune
5,Headphones,Electronics,1500,4,Delhi
6,Watch,Accessories,3000,2,Mumbai
7,Bag,Accessories,1200,3,Pune

