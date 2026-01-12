# AWS-Security
This portfolio demonstrates hands-on cloud security skills aligned with SOC Analyst / Cloud Security entry-level roles. Every project includes build steps, detections, evidence, and outcomes.

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

# Project
## Web Application
## My Draw.io Diagram
![Diagram](https://raw.githubusercontent.com/your-username/your-repo/main/Untitled%20Diagram.png)
