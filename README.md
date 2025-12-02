# 🛡️ ShadowSentry — AI-Powered Cyber Threat Intelligence Platform  

![Java](https://img.shields.io/badge/Java-17-orange?style=flat-square)
![Spring Boot](https://img.shields.io/badge/SpringBoot-3.x-brightgreen?style=flat-square)
![MongoDB](https://img.shields.io/badge/MongoDB-NoSQL-green?style=flat-square)
![React](https://img.shields.io/badge/React-Frontend-blue?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-lightgrey?style=flat-square)

---

## ⚙️ Overview  

**ShadowSentry** is an **AI-driven cybersecurity intelligence platform** that detects, analyzes, and visualizes digital breach exposure.  
It integrates real-time data from the **Have I Been Pwned (HIBP)** API and **dark-web intelligence via the TOR network** to provide users with a complete picture of their online vulnerability.  

The platform uses **Spring Boot**, **MongoDB**, and a **React-based dashboard** to deliver personalized **risk scores**, detailed **breach insights**, and **AI-generated threat reports**, helping users stay secure in an increasingly data-breach-prone world.

---

## 🚀 Features  

- 🔍 **Real-Time Breach Detection** — Fetches verified breach data via the official HIBP API.  
- 🧠 **AI-Based Risk Scoring** — Calculates exposure severity and breach frequency to assign dynamic risk levels.   
- 🧩 **Modular Microservice Design** — Separate services for feeds, incidents, and risk computation.  
- 🕵️‍♂️ **Threat Visualization Dashboard** — React UI showing risk metrics, breach history, and insights.  
- 🔐 **Secure Authentication** — JWT-based login with Spring Security and MongoDB token storage.  
- 📊 **Evidence Management** — Every breach incident is stored with timestamped metadata and evidence.  

---

## 🧠 Tech Stack  

### 🖥️ Backend  
- **Java 17 + Spring Boot 3.x**  
- **MongoDB**  
- **Spring Security & JWT Authentication**  
- **RestTemplate + HIBP API Integration**  
- **Maven** for build & dependency management  

### 💻 Frontend  
- **React (Vite)**  
- **TailwindCSS + Framer Motion**  
- **Axios** for API communication  
- **Recharts** for visual analytics  

---

                     ┌─────────────────────────────┐
                     │         Frontend            │
                     │  React + Tailwind + Axios   │
                     └────────────┬────────────────┘
                                  │
                          REST API Calls
                                  │
      ┌───────────────────────────┴───────────────────────────┐
      │                        Backend                        │
      │     Spring Boot + MongoDB + Security Layer            │
      ├───────────────────────────┬───────────────────────────┤
      │   HIBPFeedService         │   DarkWebRiskService      │
      │ (Breach incidents)        │ (TOR-based intel)         │
      └───────────────────────────┴───────────────────────────┘
                                  │
                          Breach Data & Risk Scores
                                  │
                     ┌──────────────────────────┐
                     │        MongoDB           │
                     │  Incidents & Evidence    │
                     └──────────────────────────┘



---

## ⚡ Getting Started  

### 🔧 Prerequisites  
- Java 17+  
- Node.js 18+  
- MongoDB (local or Atlas)  
- Valid **HIBP API Key**  

---

### 🛠️ Backend Setup  

```bash
# 1️⃣ Clone repository
git clone https://github.com/<your-username>/ShadowSentry.git
cd ShadowSentry/backend

# 2️⃣ Configure environment
# Edit src/main/resources/application.properties
spring.data.mongodb.uri=mongodb://localhost:27017/shadowsentry
hibp.api.key=YOUR_HIBP_KEY
hibp.baseUrl=https://haveibeenpwned.com/api/v3
app.user.agent=ShadowSentryApp/1.0

# 3️⃣ Run backend
mvn spring-boot:run

# 4️⃣Frontend Setup
-cd ../frontend
-npm install
-npm run dev

```
---

## 🔍 How It Works

- 1. User Authentication: Users register/login securely with JWT tokens.
- 2. Breach Detection: Backend queries the HIBP API for breach records linked to the user’s email.
- 3. Risk Scoring: AI model evaluates exposure level and computes a dynamic risk score.
- 4. Visualization: The React dashboard displays risk score, breach summaries, and AI insights.

---

## 👉Team Members :

A huge shoutout to our team!

- Oviya B -  https://github.com/Oviya-Babu
- Padmanathan C - https://github.com/pc3604padma
- Subashree A - https://github.com/SUBA04116
- Ramya A - https://github.com/RamyaAnandan

---


