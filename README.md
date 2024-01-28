# Introduction
This template provides a streamlined solution for automatically shutting down EC2 instances in your AWS region, promoting cost savings and resource efficiency. The template includes the essential resources and configurations for scheduled shutdowns. Notably, the flexibility of the "exception" tag allows you to exclude specific instances, tailoring the solution to your needs. Deploy effortlessly in your preferred AWS region to manage EC2 shutdowns with ease, optimizing infrastructure, reducing costs, and enhancing overall resource management.

# Pre-requisites
1. `AWS Account`
2. `EC2 Instances in Running/Stopped State`

# Steps
1. Login in to the AWS Console and search for CloudFormation
2. Click on Create stack ---> With new resources (standard) 
3. Choose Template is ready ---> Upload a template file ---> Choose file and click on Next
4. Give the stack some name ---> ec2-instance-auto-shutdown 
5. Configure the settings as per your need (optional) and click on Submit
6. Once the Stack is successfully created, click on Resources tab to view all the newly created resource (Lambda Function, IAM Role and Event Rule)
7. Now the Event Rule will trigger the Lambda function based on the cron job (by default it is MON-FRI 5 PM UTC)
8. You can also manually test the lambda function by creating a sample test event and running it.

# Screenshots
