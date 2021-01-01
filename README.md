# How Much Time Have You Spent At Work?
## This app was created on the AWS platform. It follows a serverless architecture pattern by using the following services: 

### AWS Lambda (Compute)
####  AWS Lambda is the compute layer I am using. This allows the website to function without using servers like an EC2 instance. Using AWS Lambda saves overall costs by running only when the Lambda function is triggered. This means I will not have to pay for costs when the server is idle. 

####  The app is using a Lambda function in a Python run-time environment. When the user fills out the form, the Lambda function is triggered and sends the collected data to a DynamoDB table.

### DynamoDB (Database)
#### I have chosen DynamoDB as the database because it is fully managed and offers scalabality to handle any level of traffic. It is quick to set up and integrates well with the services being used. 

### API Gateway (Networking)
#### The backend uses a RESTful API which receives the data from JavaScript executed in the browser. 

### S3 (Storage)
#### I am using S3 to store user data from DynamoDB table and for site files. 


