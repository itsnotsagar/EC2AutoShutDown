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
<img width="1152" alt="Screenshot 2024-01-28 at 9 14 09 PM" src="https://github.com/itsnotsagar/EC2AutoShutDown/assets/56265949/83ce1061-bc53-493a-a822-b27752e8a0f5">
<img width="941" alt="Screenshot 2024-01-28 at 9 42 36 PM" src="https://github.com/itsnotsagar/EC2AutoShutDown/assets/56265949/dcda0cfc-cb79-449d-9f10-287b6a1aeeab">
<img width="648" alt="Screenshot 2024-01-28 at 9 43 21 PM" src="https://github.com/itsnotsagar/EC2AutoShutDown/assets/56265949/fe3444f3-6d4d-4d64-b731-9b241a9fa7f0">
<img width="904" alt="Screenshot 2024-01-28 at 9 44 52 PM" src="https://github.com/itsnotsagar/EC2AutoShutDown/assets/56265949/e5996af4-2daa-454f-a5d6-925d24e35f13">
<img width="1146" alt="Screenshot 2024-01-28 at 9 45 15 PM" src="https://github.com/itsnotsagar/EC2AutoShutDown/assets/56265949/468c56f3-81d1-4bb5-9a3a-375631f524b1">
