# 🚀 AI Coder — Spring Boot Chatbot

> A powerful, locally-hosted AI coding assistant that helps you write, debug, and understand code — all running securely on your own machine.

---

## 📸 Preview

<img width="1920" height="947" alt="Screenshot (7808)" src="https://github.com/user-attachments/assets/6ef4367a-2e2b-459b-bc29-5c0572a5ad42" />

---

## ✨ Key Features

- 🤖 **Local AI Processing**  
  Powered by Ollama (`deepseek-coder`) — no external API calls.

- 💻 **Modern Chat UI**  
  Markdown rendering + syntax highlighting.

- 🔐 **Secure Authentication**  
  Spring Security + BCrypt password hashing.

- 🧠 **Persistent Chat History**  
  Redis-based session storage (24-hour TTL).

- ⚡ **Smart UX**  
  Typing indicator, auto-resize input, quick prompts.

- 🌐 **ngrok Ready**  
  Works with forwarded headers + CSRF protection.

---

## 🧱 Tech Stack

### 🖥️ Backend
![Spring Boot](https://img.shields.io/badge/SpringBoot-3.5.11-green?logo=spring)
![Spring AI](https://img.shields.io/badge/SpringAI-1.1.2-blue)
![Spring Security](https://img.shields.io/badge/Security-SpringSecurity-red)

### 🗄️ Database & Cache
![MySQL](https://img.shields.io/badge/MySQL-8+-blue?logo=mysql)
![Redis](https://img.shields.io/badge/Redis-Cache-red?logo=redis)

### 🤖 AI Engine
![Ollama](https://img.shields.io/badge/Ollama-LocalLLM-black)
![DeepSeek](https://img.shields.io/badge/Model-deepseek--coder-orange)

### 🎨 Frontend
![HTML](https://img.shields.io/badge/HTML5-orange?logo=html5)
![CSS](https://img.shields.io/badge/CSS3-blue?logo=css3)
![JavaScript](https://img.shields.io/badge/JS-ES6-yellow?logo=javascript)

---

## ⚙️ Prerequisites

- Java 17+
- Maven
- MySQL (3306)
- Redis (6379)
- Ollama (11434)

---

## 🔧 Installation & Setup

```bash
1️⃣ Clone Repository
git clone <your-repo-url>
cd ai-chatbot

2️⃣ Setup Ollama

ollama serve
ollama pull deepseek-coder

3️⃣ Setup MySQL
CREATE DATABASE ai_coder_db;

4️⃣ Setup Redis
redis-server

5️⃣ Configure Application

Edit:
src/main/resources/application.properties
spring.datasource.url=jdbc:mysql://localhost:3306/ai_coder_db
spring.datasource.username=root
spring.datasource.password=your_password
```
---
## ▶️ Run Application

./mvnw spring-boot:run

Windows:

.\mvnw.cmd spring-boot:run

## 🌐 Access
http://localhost:8080

---
## 🧪 Usage

Try prompts like:
```
Write a Spring Boot REST API
Debug this Java code
Explain async/await in JS
```
---
## 🧠 Architecture (Quick Insight)

```
<details> <summary>Click to expand</summary>
Spring Boot → Backend logic
Spring Security → Authentication
MySQL → User data
Redis → Chat history
Ollama → AI model
Thymeleaf + JS → UI
</details>
```

---

## 🛡️ Security

BCrypt password hashing

CSRF protection

Secure headers for ngrok

---

## 📁 Project Structure
```
ai-chatbot/
├── src/main/java/com/example/chatbot/
├── src/main/resources/
├── .env
├── pom.xml
└── docker-compose.yml
```
