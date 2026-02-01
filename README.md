# 🌦 Weather Dashboard – Serverless AWS Project

##  Project Overview

This project is a **serverless Weather Dashboard** built using AWS services.
It fetches **real-time weather data** from the OpenWeatherMap API and displays it on a web-based frontend.

The application is fully serverless, scalable, and runs within the **AWS Free Tier**.

---

## 🏗 Architecture Overview

**Flow:**

1. User enters a city name in the frontend
2. Frontend calls an API Gateway endpoint
3. API Gateway triggers an AWS Lambda function
4. Lambda fetches weather data from OpenWeatherMap
5. Lambda filters the response and returns clean JSON
6. Frontend displays formatted weather information

**Services Used:**

* AWS Amplify (Frontend Hosting)
* Amazon API Gateway (HTTP API)
* AWS Lambda (Backend Logic)
* IAM (Permissions)
* OpenWeatherMap API (External Weather Data)

---

## 🧰 Tech Stack

### Frontend

* HTML
* CSS
* JavaScript
* AWS Amplify

### Backend

* Python 3.10
* AWS Lambda
* Amazon API Gateway (HTTP API)

### Cloud & Security

* AWS IAM (Lambda Execution Role)
* CloudWatch Logs
* OpenWeatherMap API

---

## ✨ Features

* Search weather by city name
* Real-time weather data
* Clean and filtered API response
* Error handling for invalid cities
* Loading state for better UX
* Serverless and scalable architecture
* Free Tier friendly

---

## 🔐 Security Practices

* Lambda uses an **IAM execution role** (`AWSLambdaBasicExecutionRole`)
* API keys are not exposed in frontend
* (Optional Improvement) API key can be stored in **AWS Secrets Manager**

---

## 🚀 Step-by-Step Implementation

### 1️⃣ OpenWeatherMap API

* Created an OpenWeatherMap account
* Generated a free API key

### 2️⃣ IAM Role

* Created a Lambda execution role
* Attached `AWSLambdaBasicExecutionRole` for logging and permissions

### 3️⃣ AWS Lambda

* Created a Python 3.10 Lambda function
* Implemented logic to:

  * Read city from query parameters
  * Call OpenWeatherMap API
  * Handle errors
  * Filter response data
* Enabled CORS in Lambda response

### 4️⃣ API Gateway

* Created an **HTTP API**
* Connected Lambda integration
* Created GET route `/weather`
* Enabled CORS
* Deployed and obtained public endpoint

### 5️⃣ Frontend Development

* Built a simple HTML + JavaScript UI
* Used `fetch()` to call API Gateway
* Displayed weather data in readable format
* Added input validation and loading state

### 6️⃣ Hosting with AWS Amplify

* Pushed frontend code to GitHub
* Connected GitHub repo to AWS Amplify
* Deployed static website
* Accessed live public URL

---

## 🧪 How to Run the Project

1. Open the Amplify-hosted URL
2. Enter a city name (e.g., `Mumbai`)
3. Click **Get Weather**
4. View live weather details

---

## 📂 Project Structure

```
weather-dashboard/
 ├── index.html
 └── README.md
```

---

## 📈 Scalability & Cost

* Fully serverless (no servers to manage)
* Auto-scales with traffic
* Pay-per-use model
* Runs safely within AWS Free Tier

---

## 📝 Future Improvements

* Store API key in AWS Secrets Manager
* Add weather icons
* Improve UI styling
* Add caching for frequent cities
* Secure API with API Gateway API Key or Cognito

---

## 🎯 Key Learning Outcomes

* Serverless architecture on AWS
* API Gateway & Lambda integration
* External API consumption
* CORS handling
* Cloud security basics (IAM)
* Frontend ↔ Backend communication

---

## 📬 Contact

If anyone wants help with this project, feel free to contact me!

<a href="https://www.linkedin.com/in/YOUR-LINKEDIN-ID" target="_blank" style="display:inline-block; padding:10px 20px; background-color:#0A66C2; color:white; text-decoration:none; border-radius:5px; font-weight:bold;">Connect on LinkedIn</a>
