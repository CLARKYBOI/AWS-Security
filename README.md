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
%3CmxGraphModel%3E%3Croot%3E%3CmxCell%20id%3D%220%22%2F%3E%3CmxCell%20id%3D%221%22%20parent%3D%220%22%2F%3E%3CmxCell%20id%3D%222%22%20parent%3D%221%22%20style%3D%22text%3Bhtml%3D1%3BwhiteSpace%3Dwrap%3BstrokeColor%3Dnone%3BfillColor%3Dnone%3Balign%3Dcenter%3BverticalAlign%3Dmiddle%3Brounded%3D0%3Bspacing%3D7%3B%22%20value%3D%22%26lt%3Bfont%20style%3D%26quot%3Bfont-size%3A%2017px%3B%26quot%3B%26gt%3BAmplify%26lt%3B%2Ffont%26gt%3B%22%20vertex%3D%221%22%3E%3CmxGeometry%20height%3D%2230%22%20width%3D%2260%22%20x%3D%2249%22%20y%3D%22760%22%20as%3D%22geometry%22%2F%3E%3C%2FmxCell%3E%3C%2Froot%3E%3C%2FmxGraphModel%3E
