# Kafka AWS Stock Market Streamer

This project simulates real-time stock market data streaming using **Apache Kafka** and integrates it with **AWS services** for data storage, processing, and analytics. The system streams stock market data from a static dataset, processes it in real-time, and stores it in an **S3 bucket**. The data is then cataloged using **AWS Glue** and made available for querying in **Amazon Athena**.

For a detailed breakdown of the project, visit the <a href="https://devengine.notion.site/Stocks-in-Motion-Kafka-AWS-Pipeline-19c32fa5808880e992dee44407a88313?pvs=4" target="_blank">Stocks in Motion: Kafka & AWS Pipeline</a>


## Project Overview

The project consists of the following components:
1. **Kafka Producer**: Reads random rows from a stock market dataset and sends them as messages to a Kafka topic.
2. **Kafka Consumer**: Receives the messages, formats them into JSON, and stores them in an S3 bucket.
3. **AWS S3**: Acts as the storage layer for the processed data.
4. **AWS Glue**: Catalogs the data stored in S3, making it queryable in Athena.
5. **Amazon Athena**: Enables real-time querying and analysis of the stock market data.


## Architecture

![Alt Text](https://github.com/suryadeipreddyk/kafka-aws-stock-market-streamer/blob/main/Architecture.jpg)



## Prerequisites


Before running the project, ensure you have the following:
1. **AWS Account**: With access to EC2, S3, Glue, Athena, and IAM.
2. **IAM Role**: Create an IAM role with permissions for **S3**, **Glue**, and **Athena**.
3. **EC2 Instance**: For hosting Apache Kafka.
4. **Python Libraries**: Install required libraries (`boto3`, `kafka-python`, `pandas`, etc.).
5. **Dataset**: 'indexProcessed.csv'

For a detailed breakdown of the project, visit the <a href="https://devengine.notion.site/Stocks-in-Motion-Kafka-AWS-Pipeline-19c32fa5808880e992dee44407a88313?pvs=4" target="_blank">Stocks in Motion: Kafka & AWS Pipeline</a>
