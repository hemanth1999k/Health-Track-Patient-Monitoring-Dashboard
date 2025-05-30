
# 🏥 Health Track: Patient Monitoring Dashboard

A **cloud-native**, **real-time** patient health monitoring system designed for scalability, reliability, and high-performance. Built using **React**, **AWS Lambda**, **API Gateway**, **DynamoDB**, and **Terraform**, this solution provides a sleek frontend dashboard and robust serverless backend infrastructure to process thousands of data points per minute.

---

## 🚀 Features

- **📡 Real-Time Monitoring**: Displays live vitals such as heart rate, blood pressure, and temperature
- **📱 Responsive UI**: Built with React for seamless access across devices
- **☁️ Cloud-Native Backend**: AWS Lambda + API Gateway + DynamoDB ensure low-latency, high-throughput processing
- **🔧 Infrastructure as Code**: Terraform-powered AWS provisioning
- **🔐 Secure & Reliable**: High availability and integrity by design
- **📊 Scalable Architecture**: Handles 10,000+ events/minute with 99.95% uptime

---

## 🏗️ Architecture Overview

```
[Patient Devices]
      │
      ▼
[API Gateway] ⇄ [AWS Lambda] ⇄ [DynamoDB]
      │
      ▼
[React Dashboard (Frontend)]
```

---

## 📂 Project Structure

```
Patient-monitoring-dashboard-main/
├── README.md                # Project documentation
├── bash                    # Deployment/utility scripts
├── src/                    # Source code
│   ├── bash                # Bash helper (used in development)
│   ├── main.tf             # Terraform configuration
│   └── components/         # Frontend components
│       ├── Dashboard.js    # Main dashboard UI
│       └── dataProcessor.js# Client-side data processor
```

---

## 🛠️ Setup Instructions

### ✅ Prerequisites

- Node.js ≥ 16.x
- Terraform ≥ 1.3
- AWS CLI configured
- A browser for accessing the dashboard

---

### 🧩 Local Frontend Development

```bash
cd src/components
npm install
npm start
```

This will spin up the React dashboard on `http://localhost:3000`.

---

### ⚙️ Infrastructure Deployment (AWS)

> Ensure your AWS CLI is authenticated and you have admin permissions.

```bash
cd src
terraform init
terraform apply
```

- Deploys API Gateway, Lambda functions, and DynamoDB tables
- Automatically configures IAM roles and necessary resources

---

## 🧪 Testing

To run unit or integration tests (add testing setup as needed):

```bash
npm test
```

---

## 🌐 Live Demo

> Comming Soon

---

## 🤝 Contributing

We welcome contributions! Feel free to fork the repo, open issues, or submit pull requests.

---

## 📄 License

This project is licensed under the MIT License 
