## Project Description 

an event-driven application that contains an Amazon S3 bucket, an AWS Lambda function, and an Amazon DynamoDB table.
An object uploaded in the S3 bucket triggers the Lambda function, storing the object name and creation date in the DynamoDB table.

## What I have done 

To do the given task, first I started studying more about Serverless Framework and lambda functions using different websites and watched several youtube clips for the first two days. To gain more information, then I read AWS Lambda and the Serverless Framework – Hands-On Learning udemy course. The completion certificate is available using this link: 

 `https://www.udemy.com/certificate/UC-c3530026-20fd-40df-b519-6299e14ab549/`
 
To learn more about serverless and cloud formation, I also bought these two helpful udemy courses, but I have not finished them because of a shortage of time.
The courses I'm currently studying are :

1- `https://www.udemy.com/course/aws-lambda-serverless-architecture/`

   (AWS Lambda & Serverless Architecture Bootcamp, includes everything used to run a serverless stack, namely S3, Kinesis, SNS, SQS, Dynamodb, and API Gateway) 
   
2- `https://www.udemy.com/course/aws-cloudformation-master-class/`

   (AWS CloudFormation Master Class, Stephane teaches everything needed to create CloudFormation stack using Vscode)
   
In addition to youtube videos and udemy courses, I used the following website for solving some problems I faced.

`https://forum.serverless.com/`

This program resizes the PNG file formats to save more S3 bucket space, then the Lambda function triggers and records id number, creation time, name, URL, reduced size information, and update time. To run the PIL library you need to add its layer's arn to the lambda function. Depending on the region you are located in, the related arn can be found in this GitHub repository:

`https://github.com/keithrozario/Klayers`

Since I am using python 3.8 and my AWS region is eu-west-1, I added this arn to the lambda function layers (from https://api.klayers.cloud/api/v2/p3.8/layers/latest/eu-west-1/json):

`arn:aws:lambda:eu-west-1:770693421928:layer:Klayers-p38-Pillow:1`

![Serverless](https://user-images.githubusercontent.com/83725346/164093818-7f523e0c-4df3-49d0-81bc-f47e601977f9.gif)



