# 🎓 AWS Serverless Student Info App

This is a simple **serverless web app** built using AWS services that lets users **add and retrieve student information** via a form hosted on an S3 website. It follows a clean and scalable cloud architecture using fully managed AWS services.

---

## 🧰 Tech Stack

- **Frontend:** HTML, CSS, JavaScript
- **Backend:** AWS Lambda (Python)
- **API Gateway:** REST API trigger for Lambda
- **Database:** DynamoDB (On-Demand mode)
- **Hosting:** Amazon S3 (Static Website)
- **Permissions:** IAM Roles with Least Privilege

---

## 🔄 Workflow

1. User submits student data from a web form (`index.html`)
2. JS sends a POST request via API Gateway to a Lambda function
3. Lambda stores the data in DynamoDB
4. A GET request retrieves and displays student data

---

## 💸 Cost Optimization

- ✅ **DynamoDB On-Demand** (no auto-scaling, no charge if idle)
- ✅ **S3 Static Hosting** (free-tier eligible)
- ✅ **No EC2 / No VPC** used — completely **serverless & event-driven**


