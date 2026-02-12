# Digital Twin

An AI-powered Digital Twin designed as an intelligent course companion. It provides contextual responses and backend-driven processing through a scalable cloud architecture.

## 🚀 Live Deployment

Frontend is deployed and accessible at:

**[http://d1to6bbmscm3kr.cloudfront.net](http://d1to6bbmscm3kr.cloudfront.net)**

---

## 🏗 Architecture Overview

This project is deployed manually using AWS services:

* **Amazon S3** – Hosts the frontend static files and storage
* **Amazon CloudFront** – Serves the static website globally via CDN
* **AWS Lambda** – Handles backend logic
* **Amazon API Gateway** – Manages and routes API requests to Lambda

The frontend communicates with the backend through API Gateway endpoints, which trigger Lambda functions for processing.

---

## 📁 Project Structure

* `frontend/` – Frontend application
* `server.py` / backend files – FastAPI backend
* `lambda_handler.py` – Mangum adapter for AWS Lambda
* Deployment packaging handled via Docker-based Lambda build process

---

## ⚙️ Tech Stack

* FastAPI
* Mangum (for Lambda integration)
* AWS Lambda
* API Gateway
* S3
* CloudFront

---

## 📌 Notes

* Frontend is hosted as a static website via CloudFront.
* Backend is serverless and scales automatically using AWS Lambda.
* API communication is handled securely through API Gateway.

