

# AWS Step Functions for Workflow Automation

This project demonstrates how to automate a multi-step order processing workflow using **AWS Step Functions**, integrated with **AWS Lambda** and **Amazon DynamoDB**. It simulates a real-world e-commerce process using modular Lambda functions for each step—making it scalable, serverless, and easy to manage.

---

## 🚀 Project Overview

### 🧩 Workflow Components
- **OrderPlacement** – Captures order details.
- **PaymentProcessing** – Processes payment (**Currently running successfully**).
- **OrderConfirmation** – Confirms order after payment.
- **ShippingProcess** – Initiates shipping.
- **RefundHandling** – Manages refund cases.

### 🛠️ AWS Services Used
- **Step Functions** – Manages and visualizes workflow states.
- **Lambda** – Backend logic for each step.
- **DynamoDB** – Stores order and payment data (custom table name used).
- **IAM** – Provides necessary roles and permissions.
- **API Gateway** *(optional)* – For external triggering of workflows.

---

## 📌 How to Use

1. **Create DynamoDB Table**
   - Add a table with a primary key (e.g., `OrderID`) to store order data.

2. **Deploy Lambda Functions**
   - Write and deploy Lambda functions for each component:  
     `OrderPlacement`, `PaymentProcessing`, `OrderConfirmation`, `ShippingProcess`, `RefundHandling`.

3. **Define State Machine**
   - Use AWS Step Functions to define the workflow using **Amazon States Language (ASL)**.

4. **Test the Workflow**
   - Trigger the state machine manually using sample input, or connect via **API Gateway** for external integration.

---

## 🎥 Demo Video

Click below to watch the full walkthrough of the project:

https://www.youtube.com/watch?v=N_8pumQ1dB8

---

## 🧑‍💻 Getting Started

- Clone or download this repository.
- Follow the deployment steps shown in the demo video or AWS documentation.
- Make sure **IAM roles** have the necessary permissions to allow Lambda functions access to **DynamoDB** and **Step Functions**.

---

## 📬 Contact
  
For questions, feel free to open an issue or reach out via poojisrinu4@gmail.com
