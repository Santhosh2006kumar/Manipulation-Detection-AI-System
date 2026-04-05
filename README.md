# 🛡️ Manipulation Detection AI System

**Detect. Understand. Defend.**

A multi-modal AI system that detects and explains manipulative content across text, images, audio, and video — with real-time browser integration.

---

## 🚀 Overview

This project is a full-stack AI platform designed to identify emotional and persuasive manipulation in digital content.

It combines:

- 🧠 Multi-modal AI analysis  
- 🌐 Chrome extension for real-time detection  
- 📊 Analytics dashboard  
- 🧩 RAG-based memory system  

---

## ✨ Features

### 🌐 Web Application
- User authentication  
- Multi-modal input (text, image, audio, video)  
- AI-based manipulation detection  
- Interactive analytics dashboard  

---

## 📊 Dashboard

**Metrics:**
- Total analyzed  
- Manipulations detected  
- High-risk alerts  
- Average confidence  

**Charts:**
1. Detection over time  
2. Media type distribution  
3. Top manipulation techniques  
4. Risk distribution  
5. Recent activity table  

---

## 🌐 Web Application Architecture

```text
User (Web Interface)
    ↓
Frontend (HTML / CSS / JS Dashboard)
    ↓
API Layer (FastAPI Backend)
    ↓
Authentication (Login / Signup)
    ↓
Input Handling (Text / Image / Audio / Video)
    ↓
Preprocessing (OCR / Transcription / Cleaning)
    ↓
AI Engine (LLM + CLIP + Whisper)
    ↓
Manipulation Detection (Technique + Confidence + Explanation)
    ↓
Embedding Generation (MiniLM)
    ↓
Vector Database (Supabase / pgvector)
    ↓
RAG Retrieval (Past Context)
    ↓
Final Response (Personalized Output)
    ↓
Dashboard Visualization
```

---

## 🧩 Chrome Extension

- Extracts content from webpages (text, images, video)  
- Detects and highlights manipulative content  
- Displays mini dashboard with risk insights  

---

## 🧩 Chrome Extension Architecture

```text
User Browsing Webpage
    ↓
Chrome Extension (Content Script / Popup)
    ↓
Content Extraction
    ↓
- Text (DOM Parsing)
- Images
- Video / Audio
    ↓
Preprocessing
    ↓
API Call → FastAPI Backend
    ↓
AI Processing (LLM + Multi-Modal Models)
    ↓
Manipulation Detection
    ↓
Response to Extension
    ↓
UI Rendering
    ↓
- Highlight Manipulative Content
- Show Risk Score
- Mini Dashboard
```

---

## 🧩 Load Chrome Extension

* Download the  `extension_hackwell26` folder
* Open `chrome://extensions/`
* Enable **Developer Mode**
* Click **Load Unpacked**
* Select `extension_hackwell26` folder

---

## ⚙️ Tech Stack

### 🧠 AI / ML
- Mistral-7B Instruct (Fine-tuned)  
- Whisper (Speech-to-Text)  
- CLIP (Image Understanding)  
- Sentence Transformers (MiniLM)  

### 🧩 Frameworks
- LangChain  
- LangGraph  

### 🚀 Backend
- FastAPI  
- SQLAlchemy  
- Pydantic  
- Uvicorn  

### 🗄️ Database & Storage
- Supabase (PostgreSQL)  
- pgvector (Vector Search)  

### 🔐 Authentication
- Passlib (bcrypt)  

### 🌐 Frontend
- Browser Extension (JavaScript)  
- HTML5 & CSS3  

---

## 📦 Installation

### Clone the repository
```bash
git clone https://github.com/Santhosh2006kumar/Manipulation-Detection-AI-System.git
cd Manipulation-Detection-AI-System
```

### Install dependencies
```bash
pip install -r requirements.txt
```

### Run backend server
```bash
uvicorn main:app --reload
```

---

## 🔑 Environment Variables

Create a `.env` file:

```env
DATABASE_URL="postgresql://postgres:your_password.your_id.supabase.co:your_port/postgres"
OPEN_AI_API_KEY="your_openai_api_key"

YASAR_SUPABASE_URL="your_url"
YASAR_SUPABASE_KEY="your_key"

SSK_SUPABASE_URL="your_url"
SSK_SUPABASE_KEY="your_key"
```

### Notes:
- `YASAR_SUPABASE_URL/KEY` → Used for **agent memory (RAG system)**  
- `SSK_SUPABASE_URL/KEY` → Used for **authentication + logs**  
- You can use the **same Supabase project** for both  

---


## 🚀 Future Improvements
- Real-time streaming inference  
- Emotion scoring system  
- Personalized risk profiling  
- Mobile integration  

---

## 🤝 Contributing
Contributions are welcome! Feel free to fork the repo and submit a pull request.

---

## 👥 Team

- Tanusri K 
- Suganya G 
- Mohamed Yasar Arafath J
- Santhosh Kumar S
