# How Much Time Have You Spent At Work?
## I have created this app to help myself and others become more aware of how much time we spend at work. After calculating the numbers myself, I was shocked to see how much of the year I have spent at work. 
#### My intent is to find ways to optimize the time you have in your day to do other tasks.This app will include a sign up feature where users can keep track of their hours spent at their current job



## This app was created on the AWS platform. It follows a serverless architecture pattern by using the following services: 

### AWS Lambda (Compute)
####  AWS Lambda is the compute layer I have chosen to use. AWS Lambda allows the website to function without using servers like an EC2 instance. Using AWS Lambda saves overall costs by running only when the Lambda function is triggered by an event. This means I will not have to pay for costs when the server is idle which optimizes performance. 

####  The app is using a Lambda function in a Python run-time environment. When the user fills out the form, the Lambda function is triggered and writes the collected data to a DynamoDB table.

### DynamoDB (Database)
#### I have chosen DynamoDB as the database because it is fully managed and offers scalability to handle any level of traffic. It is quick to set up and integrates well with the services being used such as Lambda. 

### API Gateway (Networking)
#### The backend uses a RESTful API that triggers the Lambda function. When the user interacts with the site, this creates the event. This event receives the data from JavaScript executed in the browser. The JavaScript code is translated into JSON format and sent to Lambda for further action. 


### S3 (Storage)
#### I am using S3 to store user data from DynamoDB table and for site files. Results from CloudWatch are also stored in S3 for easier access & management


