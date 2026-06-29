# aws-cloudtrail-splunk-integration
End-to-end integration of AWS CloudTrail with Splunk Enterprise using S3, SQS and Splunk Add-on for AWS.

# AWS CloudTrail Integration with Splunk Enterprise

## Overview
This project demonstrates how to integrate AWS CloudTrail logs with Splunk Enterprise using Amazon S3, Amazon SQS, IAM Roles, and the Splunk Add-on for AWS.
The objective is to build an enterprise-style logging pipeline capable of collecting AWS audit logs for monitoring, troubleshooting, and security investigations.
---
## Architecture
AWS CloudTrail → Amazon S3 → Amazon SQS → Splunk Add-on for AWS → Splunk Index
---
## Technologies Used
* AWS EC2
* AWS IAM
* AWS CloudTrail
* Amazon S3
* Amazon SQS
* Splunk Enterprise
* Splunk Add-on for AWS
* Red Hat Enterprise Linux 9
---
## Project Objectives
* Configure AWS CloudTrail
* Deliver logs to Amazon S3
* Configure Amazon SQS notifications
* Configure IAM permissions
* Install and configure Splunk Add-on for AWS
* Ingest CloudTrail logs into Splunk
* Validate indexed events
* Create dashboards and security alerts
---
## Configuration Steps
1. Launch EC2 instance
2. Install Splunk Enterprise
3. Install Splunk Add-on for AWS
4. Configure IAM Role
5. Create CloudTrail Trail
6. Configure S3 bucket
7. Configure SQS queue
8. Configure Splunk AWS Account
9. Configure CloudTrail Data Input
10. Validate data ingestion
---
## Validation
Example SPL:
index=aws sourcetype=aws:cloudtrail
---
## Future Enhancements
* CloudWatch Logs
* VPC Flow Logs
* GuardDuty
* AWS Config
* Security Dashboards
* SOC Detection Rules
---
## Author
Shakeer Mohammed
Splunk Administrator | AWS | SIEM | Cybersecurity
