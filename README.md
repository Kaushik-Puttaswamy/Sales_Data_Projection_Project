# Sales_Data_Projection_Project

## Overview

The Sales Data Projection Project is designed to generate mock sales order data, store it in an AWS DynamoDB table, and process it using an AWS Lambda function. The goal is to simulate real-time order data processing by capturing and transforming order information for further analytics.

## Project Components

1. DynamoDB Mock Data Generator (dynamodb_mock_data_gen.py)


This script generates random order data and inserts it into a DynamoDB table named GadgetOrders.


Features:

	
 •	Generates random sales orders with orderid, product_name, quantity, and price.
	
 •	Uses boto3 to connect to AWS DynamoDB and insert records.
	
 •	Runs continuously, adding a new record every 2 seconds.
	•	Can be stopped using a manual keyboard interrupt (Ctrl + C).

Setup & Execution:
	1.	Ensure you have AWS credentials configured (aws configure).
	2.	Install dependencies:
