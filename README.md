# Yelp Dataset Analysis with Kafka and Spark

This project demonstrates how to process Yelp's academic dataset using Apache Kafka for streaming data and Apache Spark for data processing. The pipeline reads business and check-in data from JSON files, streams them through Kafka, processes them with Spark, merges the datasets, and saves the result as a JSON file.

## Why I Built This
I developed this project as part of my journey to master big data tools like Kafka and Spark. Working with Yelp's dataset was a great way to understand real-time data streaming and processing!

## Project Overview
The goal of this project is to:
1. Stream Yelp's business and check-in data using Apache Kafka.
2. Process the streamed data using Apache Spark.
3. Merge the datasets based on `business_id`.
4. Save the merged dataset as a JSON file.

The notebook (`yelp_kafka_spark.ipynb`) handles the entire pipeline, from setting up Kafka and Spark to processing and saving the data.

## Dataset
The dataset used is Yelp's Academic Dataset

The project specifically uses:
- `yelp_academic_dataset_business.json`: Contains business details like name, address, ratings, and categories.
- `yelp_academic_dataset_checkin.json`: Contains check-in timestamps for businesses.

**Note**: You need to download these files and place them in the project directory before running the notebook.

## Technologies Used
- **Apache Kafka**: For real-time data streaming.
- **Apache Spark**: For distributed data processing.
- **Python**: For scripting and data manipulation (using `kafka-python` and `pyspark` libraries).
- **Zookeeper**: For managing Kafka brokers.
- **Power BI**: For creating interactive dashboards to visualize business and check-in data.

### Prerequisites
- Python 3.7+
- Java 11 - Apache Kafka 3.9.0
- Apache Spark 3.5.5
- Internet connection (for downloading dependencies)
