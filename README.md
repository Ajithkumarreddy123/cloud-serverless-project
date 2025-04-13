# 🛒 eCommerce Analytical Platform on AWS

This project demonstrates the design and deployment of a scalable, secure, and efficient analytical platform for an eCommerce application using various AWS services.

## 🚀 Overview

The goal of this platform is to collect, store, process, and analyze eCommerce data (such as sales, customer behavior, and product insights) in real-time and batch modes, enabling business stakeholders to make data-driven decisions.

## 🧰 AWS Services Used

- **Amazon S3** – For data storage (raw, processed, and curated zones)
- **AWS Glue** – For ETL (Extract, Transform, Load) operations
- **Amazon Athena** – For querying data directly from S3
- **Amazon Kinesis** – For real-time data streaming and processing
- **AWS Lambda** – For serverless compute tasks and automation
- **Amazon QuickSight** – For building interactive dashboards and data visualizations
- **AWS IAM** – For managing access and security
- **AWS CloudWatch** – For monitoring and logging
- **Amazon DynamoDB

## 📊 Architecture Diagram
- You can see in my requiremnets files along with the  manifest files, and my project report 
  
## 🔧 Setup and Deployment

### 1. Prerequisites

- AWS Account with admin permissions
- IAM roles for Glue, Redshift, Lambda, and Kinesis
- Source data files (CSV/JSON) for simulation

### 2. Data Pipeline Flow

1. Raw data uploaded to **S3 bucket**
2. **AWS Glue Jobs** perform ETL and store processed data back in S3
3. **Athena** is used for ad-hoc querying
4. **Kinesis** ingests real-time order data and pushes to S3 or Redshift via Lambda
5. **Redshift** stores cleaned and enriched data
6. **QuickSight** connects to Redshift and S3 to visualize insights

### 3. Data Schema Examples

- **Customers**: ID, Name, Email, Join Date
- **Orders**: Order ID, Customer ID, Timestamp, Amount
- **Products**: Product ID, Category, Price

## 📈 Sample Insights

- Top 10 selling products
- Peak shopping hours
- Customer retention trends
- Sales trends by region and device

## 🛠️ Tools & Technologies

- AWS CloudFormation (optional) for infrastructure as code
- Python for Lambda scripts
- SQL for Athena and Redshift queries

## 📌 Key Features

- Scalable, serverless, and secure
- Supports both batch and real-time data pipelines
- BI-ready architecture with QuickSight dashboards
- Cost-effective and modular design

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## 📝 License

This project is licensed under the MIT License.
