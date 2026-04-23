# 🚀 AWS AI Chat Application 🤖☁️

## 📌 Project Description
The **AWS AI Chat Application** is a scalable, serverless, AI-powered chat system built using modern AWS cloud services. It allows users to send messages and receive intelligent AI-generated responses using **Amazon Bedrock** and **Amazon Q**.  

The system is designed with a secure, scalable, and cost-efficient serverless architecture using AWS best practices.

---

## 🏗️ Architecture Diagram

![Architecture Diagram](./diagrams/architecture.png)

### 📖 Architecture Overview
- User interacts with a web-based chat interface  
- Requests are routed through **Amazon API Gateway**  
- **AWS Lambda** processes the request  
- Lambda communicates with **Amazon Bedrock** and **Amazon Q** for AI responses  
- Data is stored in **Amazon DynamoDB**  
- Logs and files are stored in **Amazon S3**  
- Monitoring is handled via **Amazon CloudWatch**  

---

## ⚙️ Tech Stack

- **Frontend:** React / Web Application  
- **Backend:** AWS Lambda  
- **API Layer:** Amazon API Gateway  
- **Database:** Amazon DynamoDB  
- **Storage:** Amazon S3  
- **AI Services:** Amazon Bedrock, Amazon Q  
- **Infrastructure:** AWS Serverless Architecture  

---

## ☁️ AWS Services Used & Their Role

- **AWS IAM** → Manages authentication and access control  
- **Amazon API Gateway** → Handles incoming API requests  
- **AWS Lambda** → Executes backend business logic  
- **Amazon Bedrock** → Generates AI-powered responses  
- **Amazon Q** → Provides intelligent assistance and suggestions  
- **Amazon DynamoDB** → Stores chat history and user data  
- **Amazon S3** → Stores logs, static assets, and backups  
- **Amazon CloudWatch** → Monitoring, logging, and performance tracking  

---

## 🔄 Workflow

1. User opens the chat application  
2. User sends a message from the UI  
3. Request is sent to **API Gateway**  
4. API Gateway triggers **AWS Lambda**  
5. Lambda processes the request  
6. Lambda sends input to:
   - Amazon Bedrock (AI response generation)
   - Amazon Q (contextual assistance)
7. AI response is returned to Lambda  
8. Lambda stores chat data in **DynamoDB**  
9. Logs may be stored in **S3**  
10. Response is sent back via API Gateway to the user  

---

## ✨ Key Features

- 🤖 AI-powered intelligent chat system  
- ☁️ Fully serverless AWS architecture  
- ⚡ High scalability and performance  
- 🔐 Secure API handling with IAM  
- 📦 Persistent chat storage  
- 📡 Fast real-time responses  
- 📊 Monitoring and logging support  

---

## 💰 Cost Estimation (AWS AI Chat App)

This is a **serverless pay-as-you-go project**, so cost depends on usage.

---

### ⚙️ AWS Services Cost

- **AWS Lambda:** $0 – $5/month (free tier available)
- **API Gateway:** $1 – $10/month (depends on API calls)
- **Amazon Bedrock:** $5 – $50+ /month (main cost, based on AI tokens)
- **Amazon Q:** $0 – $20/month (low usage)
- **DynamoDB:** $1 – $5/month (free tier available)
- **Amazon S3:** $0 – $2/month (very low storage cost)
- **CloudWatch:** $1 – $5/month (logs & monitoring)

---

## 💡 Total Estimated Cost

- 🟢 Free Tier: **$0 – $10/month**
- 🟡 Small Project: **$10 – $40/month**
- 🔴 Medium Usage: **$50 – $150/month**

---

## ⚡ Key Insight
Most cost comes from **Amazon Bedrock (AI usage)**, while other services are low-cost in serverless architecture.

