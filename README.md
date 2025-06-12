# Student Info Cloud App 🚀

A simple AWS-powered web application to collect and view student data using a serverless architecture.

## 🛠 Tech Stack

- **Frontend:** HTML, CSS, JavaScript
- **Backend:** AWS Lambda (Python)
- **API Gateway:** Handles POST/GET HTTP requests
- **Database:** DynamoDB
- **Hosting:** Amazon S3 (static website hosting)

## 📦 Features

- Collects student details (name, roll number, etc.)
- Sends data to Lambda via API Gateway
- Stores and retrieves data from DynamoDB
- Displays stored student data on the webpage

## 🔧 AWS Services Used

| Service        | Purpose                           |
|----------------|-----------------------------------|
| S3             | Host static website               |
| API Gateway    | REST API to trigger Lambda        |
| Lambda         | Handle POST/GET logic             |
| DynamoDB       | Store student data (NoSQL table)  |
| IAM            | Permissions for Lambda/API access |

## 💸 Cost Optimization

- **On-Demand DynamoDB:** No auto-scaling costs
- **Free-tier usage:** Fully deployable with zero billing if idle
- **No running EC2 or containers**



