# 🛡️ AWS-Security
This portfolio will be documentation of my AWS learning and using it as a textbook!
### 👤 Account creation

I started with securely provisioning and hardening my AWS account
- Enabled MFA on the AWS root account, Then created a non-root IAM administrator user for my day-to-day use
- Assigned IAM users to permission-scoped IAM groups representing employee job functions, enforcing the Principle of Least Privilege (PoLP)


## 🗂️Projects
---
## ☁️ AWS Web Application
This was a simple Web Application integrating AWS services - **Amplify, Lambda, IAM, API Gateway, and DynamoDB** - to build a functional web application from scratch.
Its use was to familize my self with common AWS services and allow my self to experiece building an application.

### 🧠**Thought process**
-----
**1.** Needs a way to create/host a webpage    
**2.** Needs a way to invoke a Python functionality  
**3.** Needs a way to run code  
**4.** Needs a place to store/return output  
**5.** Needs a way to handle permission  

### 💡 Solutions
-----
**1.** **Amplify** can be used to build and host websites. (For simplicity, a text editor was used to create an index.html page)  


**2.** **API Gateway** can be used to build a REST API to invoke the Lambda function.  


**3.** **Lambda** running Python code serverlessly upon some trigger. (In this case, it was user input)  


**4.** **DynamoDB** used a key-value ("NoSQL") database. (This wasn't needed because I could have returned the value, and there was no need to store; however, for learning purposes I added it in)  


**5.** **IAM** is needed to set permissions on the execution role for Lambda



## 🗺️ Architecture Diagram
![image alt](https://github.com/CLARKYBOI/AWS-Security/blob/09aaeecd4bd1b2891cc977be899462ce9b9f1c42/Untitled%20Diagram.drawio.png)
---
## ⚛️ React App

This project is a React-based web application deployed on AWS using AWS Amplify. The frontend was clone from an existing repositiory and customized locally, including the creation fo account and sign-in pages. Backend resources are developed and tested using AWS Amplify Sandbox, allowing backend changes to be applied to a sandbox environment during development

### 🎯 Purpose
The purpose of this project was to learn frontend deployment workflows using AWS Amplify Hosting and to experiment with backend development using Amplify Sandbox. Frontend updates were deployed via repository pushes, while backend changes are applied manually within the sandbox environment
## Diagram
![image alt](https://github.com/CLARKYBOI/AWS-Security/blob/1719739d43fa4f2db9ee385952899d5824b44bab/React%20%20app.drawio.png)
## Quick Documentation / Note
## **Please Disregard below**

CLI command to change username - **aws iam update-user --user-name NAME --new-user-name NEWNAME**
  - User will stay in group but permissions will not transfer and will have to be reassigned to the new name
### Elastic Beanstalk
**Service Role** - IAM role that EB assumes to interact with other AWS services
  - Create EC2 instances, load balancers, Auto Scaling groups

**EC2 Instance Profile** - IAM role attached to the EC2 instance 
  - Giving permissions for applications on those instances to interact with other AWS services
      - Allowing to upload logs to S3, write to an RDS DB and Cloudwatch

### AWS Lambda 
  - Code runs on a server that is not needed to be managed and runs in response to some event

### S3 
 - Object storage storing data within buckets identified by a unique key and supported by metadata
