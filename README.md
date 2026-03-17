# 🏙️ Real-Time Urban Data Integration and Analytics Platform for Smart City Applications

![Python](https://img.shields.io/badge/Python-3.10-blue)
![DeepSeek](https://img.shields.io/badge/Model-DeepSeek--R1%3A7B-green)
![Ollama](https://img.shields.io/badge/Framework-Ollama-orange)
![Open-Meteo](https://img.shields.io/badge/API-Open--Meteo-lightblue)
![OpenAQ](https://img.shields.io/badge/API-OpenAQ-red)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)

---

## 📌 Project Overview

This project is a **Real-Time Urban Data Integration and Analytics Platform** 
built for Smart City Applications. It uses an **Agentic AI framework** powered 
by **DeepSeek-R1:7B** (via Ollama) to intelligently process real-time urban 
data queries including weather and air quality information.

---

## 👥 Team 4

| Name | Role |
|------|------|
| Kritika Gupta | Backend, API Integration, Analytics |
| Rohit Manohar Saggam | AQI Agent, Data Integration, Testing |
| Nandini Devi Poreddy | DeepSeek Setup, UI Components, Insights |

**Faculty Mentor:** Dr. Razi Iqbal  
**Instructor:** Dr. Michael Johnson  
**Course:** CPS698 Capstone Project

---

## 🗂️ Project Structure
```
smart-city-analytics-platform/
│
├── README.md
├── requirements.txt
│
├── week6/        # Project Setup, Research & Architecture
├── week7/        # Tool Agent Development & Data Integration
├── week8/        # UI Layer, Response Generation & Analytics
└── docs/         # Diagrams, architecture, meeting notes
```

---

## ⚙️ Tech Stack

| Component | Technology |
|-----------|------------|
| AI Model | DeepSeek-R1:7B |
| LLM Framework | Ollama |
| Runtime | Google Colab (GPU T4) |
| Weather API | Open-Meteo |
| Air Quality API | OpenAQ |
| Language | Python 3.10 |
| Agentic Pattern | Tool-calling / Function-calling Agent |

---

## 📅 Weekly Progress

### ✅ Week 6 — Project Setup, Research & Architecture
| Card | Owner | Status |
|------|-------|--------|
| Backend & Environment Setup | Kritika | ✅ Done |
| DeepSeek Model & Agentic Framework Setup | Nandini | ✅ Done |
| API Access Setup (Open-Meteo & OpenAQ) | Kritika | ✅ Done |
| Proof of Concept – Tool Calling | Rohit | ✅ Done |
| Research on Agentic AI Patterns | Rohit | ✅ Done |
| System Architecture Diagram | All Members | ✅ Done |
| MVP API Prototype | Kritika | ✅ Done |
| User Interaction Flow Design | Nandini | ✅ Done |
| Weekly Team Sync & Documentation | All Members | ✅ Done |

### ✅ Week 7 — Tool Agent Development & Data Integration
| Card | Owner | Status |
|------|-------|--------|
| Weather Tool Agent | Kritika | ✅ Done |
| AQI Tool Agent | Rohit | ✅ Done |
| Dynamic Location-Based Retrieval | Nandini | ✅ Done |
| Unified Data Integration Layer | Rohit | ✅ Done |
| Intent Classification Module | Kritika | ✅ Done |

### ✅ Week 8 — UI Layer, Response Generation & Analytics
| Card | Owner | Status |
|------|-------|--------|
| Basic UI/CLI for Query Input | Kritika | ✅ Done |
| Display Components | Nandini | ✅ Done |
| Natural Language Response Generator | Kritika | ✅ Done |
| End-to-End Flow Integration | Rohit | ✅ Done |
| Edge Case Testing | Nandini | ✅ Done |
| Trend Detection Logic | Kritika | ✅ Done |
| Daily/Hourly Summary APIs | Rohit | ✅ Done |
| Insight Generation | Nandini | ✅ Done |
| Analytics Integration | Rohit | ✅ Done |
| Analytics Testing | Kritika | ✅ Done |

---

## 🤖 Proof of Concept — Temperature Agent (Week 6)

### Agentic Loop:
```
User Query
    ↓
DeepSeek-R1:7B (Reasoning)
    ↓
Tool Call → get_temperature(city)
    ↓
Open-Meteo API (Real-Time Data)
    ↓
DeepSeek-R1:7B (Final Response)
    ↓
Structured Weather Report
```

---

## 🚀 How to Run

1. Open `week6/temp_agent.ipynb` in **Google Colab**
2. Set runtime to **GPU (T4)**
3. Run all cells from top to bottom
4. Use the interactive mode in the last cell to query any city

---

## 📎 Resources

- [Open-Meteo API Docs](https://open-meteo.com/en/docs)
- [OpenAQ API Docs](https://docs.openaq.org)
- [Ollama](https://ollama.com)
- [DeepSeek Model](https://ollama.com/library/deepseek-r1)
- [Project Trello Board](https://trello.com/b/gq3GgqV9/team-4-real-time-urban-data-integration-and-analytics-platform-for-smart-city-applications) 
---

## 📝 License
Academic project — Central Michigan University, CPS698 Capstone Project
