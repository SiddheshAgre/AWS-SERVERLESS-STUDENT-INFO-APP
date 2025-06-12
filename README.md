#  AWS Serverless Student Info App

This is a simple serverless web application built using AWS services that allows you to:

✅ Add student details  
✅ View all student records  
✅ Store data securely using DynamoDB  
✅ Interact via API Gateway and Lambda  
✅ Host static frontend on S3

---

## 🚀 Tech Stack

| Layer      | Service Used              |
|------------|---------------------------|
| Frontend   | HTML, CSS, JavaScript     |
| Hosting    | Amazon S3 (Static Website)|
| Backend    | AWS Lambda (Python)       |
| API Layer  | Amazon API Gateway        |
| Database   | Amazon DynamoDB           |

---

## 🧩 Architecture

```plaintext
User ↔️ HTML Form (S3) ↔️ API Gateway ↔️ Lambda ↔️ DynamoDB
```

---

## 🛠️ Features

- 🔄 Add student info (ID, Name, Class, Age)
- 👀 View all student records
- 🌐 Serverless and scalable
- 🆓 Runs on AWS Free Tier

---

## 🗃️ DynamoDB Schema

| Attribute  | Type   |
|------------|--------|
| studentid  | String (Partition Key) |
| name       | String |
| class      | String |
| age        | Number |

---

## 📁 Project Structure

```
├── index.html          # Web UI form
├── scripts.js           # API calls (GET/POST)
├── insertStudent.py      # Lambda for inserting data
├── getStudent.py.py       # Lambda for fetching data
```

---

## 📦 How It Works

1. User fills form on static website hosted in S3  
2. JavaScript sends request to API Gateway  
3. API triggers Lambda (POST → insert, GET → fetch)  
4. Lambda interacts with DynamoDB table `studentData`  
5. Data is stored and retrieved securely  

---

## 🌍 Live Demo

If hosted publicly, add the link here like:

🔗 [View Demo](http://serverless-website-bucket-project.s3-website.ap-south-1.amazonaws.com)

---

## 🧾 Sample JSON

```json
{
  "studentid": "123",
  "name": "John Doe",
  "class": "10",
  "age": 16
}
```

---

## 🔐 IAM Policies Used

- `dynamodb:PutItem`  
- `dynamodb:GetItem`  
- `dynamodb:Scan`  
- `lambda:InvokeFunction`  

---

## 🧠 Learning Outcome

- Practical experience with AWS Lambda, DynamoDB, and API Gateway  
- Built real-world serverless architecture  
- Learned how to deploy a frontend via S3  

---
