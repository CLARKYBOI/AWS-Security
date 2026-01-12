# AWS-Security
This portfolio demonstrates hands-on cloud security skills aligned with SOC Analyst / Cloud Security entry-level roles. Every project includes build steps, detections, evidence, and outcomes.


## Projects
[AWS Web Application](#diagram)
This was a simple Web Application integrating AWS services - **Amplify, Lambda, IAM, API Gateway, and DynamoDB** - to build a functional web application from scratch.
Its use was to familize my self with common AWS services and allow my self to experiece building an application

🧠**Thought process**
1. Needs way to create/host a webpage  
2. Needs way to invoke a python functionality  
3. Needs a way to run code  
4. Needs a place to store/return output  
5. Needs a way to handle permission  


#### Diagram
![image alt](https://github.com/CLARKYBOI/AWS-Security/blob/09aaeecd4bd1b2891cc977be899462ce9b9f1c42/Untitled%20Diagram.drawio.png)



## Quick Documentation / Note
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
