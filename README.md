# How Much Time Have You Spent At Work?
## This app was created and is hosted on AWS. It follows a serverless architecture pattern by using the following services: 
### AWS Lambda (Compute)
#### - AWS Lambda is the compute layer I am using. This allows the website to function without using servers like an EC2 instance. Using AWS Lambda saves overall costs by running only when the Lambda function is triggered. This means I will not have to pay when the server is idle. 
#### - The app is using a Lambda function in a Python run-time environment. When the user fills out the form, the Lambda function is triggered and sends the collected data to a DynamoDB table.

###  DynamoDB (Database)
#### 
### - API Gateway (Networking)
### - S3 (Object Storage)
### - Route 53(Networking)
### - CloudWatch(Monitoring)

