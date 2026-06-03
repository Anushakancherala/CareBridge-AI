# CareBridge AI 🏥🤖

An AI-powered elderly care platform that helps caregivers remotely monitor and support elderly parents through personalized WhatsApp interactions, medication tracking, health monitoring, and intelligent risk detection.

---

## 📌 Overview

CareBridge AI is a full-stack healthcare companion platform designed for families whose elderly parents live alone or far away.

The platform combines:

* WhatsApp-based health check-ins
* Medication reminders
* Daily wellness tracking
* AI-powered risk detection
* Personalized relationship memory

Unlike traditional reminder applications, CareBridge AI remembers routines, preferences, and past conversations to create a more human and supportive experience.

---

## 🎯 Problem Statement

Many elderly individuals face:

* Missed medications
* Irregular meals
* Lack of daily monitoring
* Social isolation
* Delayed health issue detection

Caregivers often struggle to stay informed about their parents' well-being when living in different cities or countries.

---

## 💡 Solution

CareBridge AI acts as an intelligent healthcare companion that:

* Sends daily WhatsApp check-ins
* Tracks medication adherence
* Monitors meals, hydration, and wellness
* Processes voice responses
* Detects health risks
* Alerts caregivers when intervention is needed
* Personalizes conversations using relationship memory

---

## ✨ Key Features

### 📱 WhatsApp Integration

* Automated daily reminders
* Interactive Yes / No responses
* Voice note support

### 💊 Medication Tracking

* Multiple medications per parent
* Scheduled reminders
* Adherence monitoring

### 🧠 AI-Powered Risk Detection

* Medication compliance analysis
* Mood tracking
* Meal tracking
* Risk score generation

### ❤️ Relationship Memory

* Stores preferences and routines
* Remembers family events
* Generates personalized messages

### 🎙️ Voice Note Processing

* Speech-to-text transcription
* Natural language processing
* Automatic memory extraction

### 📊 Caregiver Dashboard

* Parent monitoring
* Health trends
* Alert management
* Health reports

---

## 🏗️ System Architecture

```text
Caregiver Dashboard (Next.js)
            │
            ▼
      FastAPI Backend
            │
            ▼
     LangGraph Agents
            │
 ┌──────────┼──────────┐
 ▼          ▼          ▼
Risk      Memory    Wellness
Agent     Agent      Agent
            │
            ▼
      PostgreSQL
            │
            ▼
      Twilio WhatsApp
            │
            ▼
       Elderly User
```

---

## 🤖 Multi-Agent Architecture

### 1. Medication Agent

Tracks medication schedules and adherence.

### 2. Wellness Agent

Analyzes meals, hydration, and wellness activities.

### 3. Risk Detection Agent

Calculates health risk scores.

### 4. Health Summary Agent

Generates weekly and monthly summaries.

### 5. Relationship Memory Agent

Stores personal memories and preferences.

### 6. Notification Agent

Sends caregiver alerts and reminders.

---

## 🛠️ Tech Stack

### Frontend

* Next.js 14
* TypeScript
* Tailwind CSS
* Zustand

### Backend

* FastAPI
* Python
* SQLAlchemy
* APScheduler

### Database

* PostgreSQL

### AI & Automation

* LangGraph
* OpenAI GPT-4o
* Whisper Speech-to-Text

### Authentication

* Clerk JWT
* Google OAuth

### Communication

* Twilio WhatsApp API

---

## 📂 Project Structure

```text
CareBridge-AI/
│
├── frontend/
│   ├── app/
│   ├── components/
│   ├── hooks/
│   └── types/
│
├── backend/
│   ├── app/
│   ├── agents/
│   ├── models/
│   ├── routers/
│   ├── services/
│   └── tests/
│
├── docs/
├── README.md
└── LICENSE
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/your-username/CareBridge-AI.git
cd CareBridge-AI
```

### Backend Setup

```bash
cd backend

python -m venv .venv

# Windows
.venv\Scripts\activate

pip install -r requirements.txt

uvicorn app.main:app --reload
```

Backend URL:

```text
http://127.0.0.1:8000
```

Swagger Documentation:

```text
http://127.0.0.1:8000/docs
```

---

### Frontend Setup

```bash
cd frontend

npm install

npm run dev
```

Frontend URL:

```text
http://localhost:3000
```

---

## 🔒 Security

* Clerk Authentication
* JWT Authorization
* Twilio Webhook Validation
* Environment-based Secrets Management
* PostgreSQL Data Protection
* Rate Limiting
* Audit Logging

---

## 🧪 Future Roadmap

* Multilingual Support
* GPT-4o Personalization
* Voice Responses
* Family Group Alerts
* Wearable Integration
* IoT Health Monitoring
* Fall Detection
* Smart Pill Box Integration

---

## 📈 Impact

CareBridge AI aims to reduce caregiver stress while improving elderly well-being through continuous monitoring, personalized communication, and intelligent health risk detection.

---

## 👩‍💻 Author

**Anusha Kancherala**

Passionate about AI Engineering, Full-Stack Development, Agentic AI Systems, and Healthcare Technology.

---

## ⭐ Support

If you found this project useful, consider giving it a star on GitHub.
