# Hive vs. Spark Speed Comparison Project

## Overview
Led a comprehensive analysis to compare the performance of Apache Hive and Apache Spark within the Hadoop ecosystem, focusing on processing and querying large datasets. The project aimed to determine the most efficient technology for a small to mid-cap e-commerce business, considering the current infrastructure and dataset size.

## Firm Context
- **Firm Size:** Small to mid-cap
- **Sector:** E-commerce
- **Competitors:** Amazon, eBay, Alibaba, JD.com, AliExpress, Wish, Shopify, and Coupang

## Human Capital Requirements
- **Personnel:** 1-2 people
- **Skills Required:** Data cleaning, data mining, data visualization
- **Training Duration:** 5 weeks

## Technologies Used
- **Google Cloud Platform (GCP):** Managed infrastructure and data storage.
- **Apache Hive (Hive2, Hive Metastore):** Schema creation and query execution.
- **Apache Spark:** In-memory data processing for high-speed querying.
- **Hadoop Distributed File System (HDFS):** Distributed data storage.
- **YARN:** Resource management for cluster operations.
- **HQL (Hive Query Language):** Query language for Hive.
- **OpenRefine:** Data cleaning and transformation.
- **Excel:** Data preprocessing and manual adjustments.

## Key Steps

### 1. Data Preparation
- **Cleaning and Formatting:** Processed the dataset by removing whitespace in Excel and eliminating commas in product names using OpenRefine’s replace function.
- **Data Upload:** Created a project and bucket in Google Cloud Platform (GCP), uploading the cleaned dataset to ensure secure and efficient data handling.

### 2. Cluster and Data Management
- **Cluster Setup:** Deployed a Hadoop cluster on GCP with 1 master node and 2 worker nodes, establishing SSH access for seamless cluster interaction.
- **Data Handling:** Successfully transferred the dataset from GCP storage to HDFS, optimizing it for distributed processing.

### 3. Schema and Query Design in Hive
- **Simple Schema Creation:** Initiated the project by creating a basic schema in Hive to test Metastore functionality.
- **Complex Schema Development:** Advanced the project by developing a complex schema tailored to the dataset’s needs.
- **Query Execution:** Ran multiple queries to analyze top customer-residing states and top-selling zip codes, benchmarking Hive’s performance.

### 4. Spark Implementation
- **Spark SQL Setup:** Configured Spark SQL to perform the same queries executed in Hive, enabling a direct performance comparison.
- **Query Execution:** Executed and analyzed queries in Spark, focusing on speed and efficiency.

## Speed Test and Performance Analysis

### First Query Speed Test
- **Hive:** Demonstrated significant performance improvements, with query times reducing from 28.7 seconds to 1.8 seconds.
- **Spark:** Initially faster at 20.6 seconds but showed less improvement, with final times at 7.4 seconds.

### Second Query Speed Test
- **Hive:** Consistent performance, ranging from 17.6 seconds to 7.0 seconds.
- **Spark:** Slightly faster, with times from 17.7 seconds to 6.8 seconds.

## Conclusion
Spark’s in-memory processing provided an initial speed advantage, but the dataset size limited the overall difference in performance. Hive’s efficiency gains over repeated queries make it a strong choice for the current data scale.

## Results and Recommendations
- **Performance Insights:** Spark showed a 28.2% initial speed advantage, but Hive outperformed in subsequent rounds with a 93.7% reduction in query time. The relatively small dataset size minimized the performance gap between the two.
- **Recommendation:** Continue using Hive for current operations, with a future transition to Spark considered if data size increases significantly or if more complex queries are required.
