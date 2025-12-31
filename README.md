# 🔍 TruthLens — Spam & Non-Spam Advertisement Classifier

**TruthLens** is an intelligent AI agent built using **Google ADK** to classify advertisements and text messages as **Spam** or **Non-Spam**, helping users identify misleading, fraudulent, or unwanted content.

This project was built as part of **Code Vipassana – Build & Blog**, held at **Google Bangalore**, with a focus on designing scalable, production-ready AI agents.

---

## 🚀 Features

- 🤖 **Google ADK–based Agent** for intelligent text classification  
- 🛡️ Detects **spam, scams, and misleading advertisements**
- ⚙️ **Microservice architecture** with independent deployments
- 🐳 **Dockerized** services for portability and scalability
- 📈 **Elasticity testing** to evaluate performance under load
- 🔌 **Ollama-powered LLM backend** for private, local inference

---

## 🧠 Architecture Overview

TruthLens follows a **decoupled architecture**:

### 1️⃣ ADK Agent Service
- Handles user requests
- Applies spam classification logic
- Exposes APIs via **FastAPI**
- Can scale independently

### 2️⃣ Ollama Backend
- Hosts the LLM model
- Dedicated inference service
- Keeps inference local and cost-efficient

---

## 📁 Project Structure


```
TruthLens/
├── README.md                    
├── ollama-backend/              # Ollama backend (separate deployment)
│   └── Dockerfile               # Backend container
└── adk-agent/                   # ADK agent (separate deployment)
    ├── pyproject.toml           # Python dependencies
    ├── env.template             # Environment template
    ├── server.py                # FastAPI server 
    ├── Dockerfile               # Container config 
    ├── elasticity_test.py       # Elasticity testing
    └── production_agent/        # Agent implementation
        ├── __init__.py          # Package init
        └── agent.py             # Agent logic
```


---

## 🛠️ Tech Stack

- **Google ADK**
- **Python**
- **FastAPI**
- **Ollama**
- **Docker**
- **LLM-based Text Classification**

---





