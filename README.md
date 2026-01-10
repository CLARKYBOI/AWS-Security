# AWS-Security
This portfolio demonstrates hands-on cloud security skills aligned with SOC Analyst / Cloud Security entry-level roles. Every project includes build steps, detections, evidence, and outcomes.

## Quick Documentation / Note
CLI command to change username - **aws iam update-user --user-name NAME --new-user-name NEWNAME**
  - User will stay in group but permissions will not transfer and will have to be reassigned to the new name
### Elastic Beanstalk
Service Role - IAM role that EB assumes to interact with other AWS services

EC2 Instance Profile - IAM role attached to the EC2 instance 
  - Giving permissions for applications on those instances to interact with other AWS services
