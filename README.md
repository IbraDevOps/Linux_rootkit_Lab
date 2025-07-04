Secure & Scalable Healthcare Data Management System on AWS

This project presents a cloud-native healthcare data management system built entirely on Amazon Web Services (AWS). It focuses on security, scalability, and compliance with healthcare industry standards by leveraging a modern AWS architecture.

Detailed technical walkthrough and implementation steps available on Medium:
 [Read the full blog](https://medium.com/p/d622bfebb045/)



Project Overview

This system demonstrates how to securely manage and scale sensitive patient records using AWS-native tools and best practices.

Architecture Highlights

Amazon EC2: Hosts a FastAPI backend for managing patient data
Amazon RDS (MySQL/PostgreSQL): Secure, scalable structured data storage
Amazon S3: Encrypted storage for patient documents and medical reports
AWS Lambda: Serverless processing and logging for upload events
Amazon CloudFront + S3: Static frontend delivery
AWS IAM: Role-based access control
CloudWatch + AWS Config: Logging, alerting, and compliance auditing



Tech Stack

Python (FastAPI) for backend APIs
MySQL/PostgreSQL on RDS for relational storage
HTML/CSS/JS** frontend served via S3 & CloudFront
AWS SDK (boto3) for interacting with AWS services



 Features

 Role-based user access with AWS IAM
 Encrypted S3 storage with restricted access
Real-time upload tracking using S3 events and Lambda
 Secure backend with parameterized SQL queries
 Full audit trail and monitoring with CloudWatch



 Repository Structure (simplified)


/secure-healthcare-aws
├── app.py                # FastAPI backend
├── requirements.txt      # Python dependencies
├── lambda/               # AWS Lambda function code
├── frontend/             # Static frontend (HTML/JS)
├── README.md




 ⚠️ Disclaimer

This is a **learning project** designed for educational and demo purposes. It is not production-ready for handling real healthcare data unless properly audited and reviewed for compliance (e.g., HIPAA).



 Author

Ibrahim Sheikh
Cloud Security Enthusiast
GitHub: [@IbraDevOps](https://github.com/IbraDevOps)
Medium: [Read more](https://medium.com/p/d622bfebb045/)
