# AWS Systems Engineer - Technical Assessment

## Architecture Overview
The solution implements a fault-tolerant, scalable web application with the following features:
- Multi-tier architecture with public and private subnets.
- Auto Scaling and an Application Load Balancer.
- RDS in Multi-AZ configuration.
- S3 for static assets.
- CI/CD with AWS CodePipeline.
- Monitoring using CloudWatch.

## Setup Instructions
1. Deploy the CloudFormation template in `infrast/temp1.yaml`.
2. Configure CodePipeline using `cicd/codepipeline.yaml`.
3. Upload your source code to the specified S3 bucket.
4. Validate the CloudFormation template as part of the CI/CD process.
5. Monitor performance using CloudWatch dashboard and alarms.

## Assumptions
- IAM roles and policies are pre-configured.
- Placeholder values are used for sensitive data.

## Security Considerations
- Security Groups restrict access to resources.
- RDS is in a private subnet.

## Scaling Strategy
- Auto Scaling adjusts the instance count based on load.

## Improvements
- Add more detailed monitoring for database performance.
- Implement HTTPS for the Load Balancer.
