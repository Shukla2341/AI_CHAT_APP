# 🚀 AWS AI Chat Application 🤖☁️

## 📌 Project Description
The **AWS AI Chat Application** is a scalable, serverless AI-powered chat system hosted using **Amazon S3 Static Website Hosting** for the frontend and powered by AWS backend services.  

Users interact through a simple HTML-based chat interface, and all messages are processed using **Amazon Bedrock AI models** to generate intelligent responses.

This architecture follows AWS serverless best practices for scalability, security, and low cost.

---

## 🏗️ Architecture Diagram

![Architecture Diagram](./diagrams/architecture.png)

### 📖 Architecture Flow Overview

- Frontend is hosted as a **static website on Amazon S3**
- User sends message from HTML chat UI
- Request is sent to **Amazon API Gateway**
- API Gateway triggers **AWS Lambda**
- Lambda processes request and sends it to **Amazon Bedrock**
- Bedrock generates AI response
- Lambda stores chat history in **Amazon DynamoDB**
- Logs and files are stored in **Amazon S3**
- Response is returned back to the frontend

---

## 🔄 Workflow

1. User opens chat UI (HTML page hosted on S3)
2. User types a message and clicks send
3. Request goes to **API Gateway**
4. API Gateway triggers **AWS Lambda**
5. Lambda forwards request to **Amazon Bedrock**
6. Bedrock generates AI response
7. Lambda stores chat in **DynamoDB**
8. Response is sent back to frontend
9. User sees AI reply in browser

---

## ⚙️ Tech Stack

- **Frontend:** HTML, CSS, JavaScript (Hosted on S3)
- **Backend:** AWS Lambda  
- **API Layer:** Amazon API Gateway  
- **Database:** Amazon DynamoDB  
- **Storage:** Amazon S3  
- **AI Engine:** Amazon Bedrock  
- **Infrastructure:** AWS Serverless Architecture  

---

## ☁️ AWS Services Used & Their Role

- **Amazon S3** → Hosts static frontend (HTML chat UI) + stores files  
- **Amazon API Gateway** → Handles HTTP requests from frontend  
- **AWS Lambda** → Backend logic and request processing  
- **Amazon Bedrock** → AI response generation (core intelligence)  
- **Amazon DynamoDB** → Stores chat history  
- **AWS IAM** → Security and permissions management  
- **Amazon CloudWatch** → Monitoring and logging  

---

## ✨ Key Features

- 🤖 AI-powered chat using Amazon Bedrock  
- 🌐 Fully static frontend hosted on S3  
- ⚡ Serverless backend (no server management)  
- 🔐 Secure AWS IAM-based access control  
- 📦 Chat history storage in DynamoDB  
- 📡 Fast API-based communication  
- ☁️ Highly scalable and cost-efficient system  

---

## 💰 Cost Estimation (AWS AI Chat App)

This project follows a **serverless pay-as-you-go model**.

### ⚙️ AWS Services Cost

- **Amazon S3 (Frontend Hosting):** $0 – $2/month  
- **AWS Lambda:** $0 – $5/month  
- **API Gateway:** $1 – $10/month  
- **Amazon Bedrock:** $5 – $50+ /month (main cost)  
- **DynamoDB:** $1 – $5/month  
- **CloudWatch:** $1 – $5/month  

---

## 💡 Total Estimated Cost

- 🟢 Free Tier: **$0 – $10/month**  
- 🟡 Small Project: **$10 – $40/month**  
- 🔴 Medium Usage: **$50 – $150/month**

---

## ⚡ Key Insight
The main cost driver is **Amazon Bedrock (AI model usage)**, while S3-hosted frontend and other services remain low-cost in this serverless architecture.
