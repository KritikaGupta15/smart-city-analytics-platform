# Week 6 — Project Setup, Research & Architecture

> **Course:** CPS698 Capstone Project
> **Team 4:** Kritika Gupta | Rohit Manohar Saggam | Nandini Devi Poreddy
> **Mentor:** Dr. Razi Iqbal | **Instructor:** Dr. Michael Johnson

## 📌 Overview
Week 6 focused on setting up the full project foundation — environment, tools, APIs, and a working proof of concept using an Agentic AI framework powered by DeepSeek-R1:7B.

## ✅ Completed Cards

### Card 1: Backend & Environment Setup — Kritika
- Created shared GitHub repository for version-controlled collaboration
- Set up Google Colab environment with GPU (T4) runtime
- Installed Ollama, zstd, and all required Python libraries
- Configured isolated environment to avoid dependency conflicts

### Card 2: DeepSeek Model & Agentic Framework Setup — Nandini
- Downloaded and configured DeepSeek-R1:7B model via Ollama
- Started Ollama server in background using subprocess
- Verified model responds correctly to test prompts
- Built basic agent class structure for tool routing and reasoning

### Card 3: API Access Setup (Open-Meteo & OpenAQ) — Kritika
- Studied Open-Meteo Geocoding and Weather API endpoints
- Sent trial requests and verified valid JSON responses
- Identified key fields: temperature, humidity, wind speed, timestamps
- Documented API constraints and geographic input formats

### Card 4: Proof of Concept – Tool Calling — Rohit
- Built get_temperature() function calling Open-Meteo API in real-time
- Validated that DeepSeek can generate structured tool calls
- Tested with 4 different natural language queries
- Confirmed output matches expected schema (function name + arguments)

### Card 5: Research on Agentic AI Patterns — Rohit
- Explored multi-agent coordination patterns (reasoning + tool agents)
- Studied best practices for tool routing and multi-step reasoning
- Documented agentic design principles for team alignment
- Identified intent-to-tool mapping strategies

### Card 6: System Architecture Diagram — All Members
- Identified all major modules: reasoning agent, tool agents, backend, APIs, UI
- Illustrated query flow from user input to final response
- Produced labeled diagram for project report

### Card 7: MVP API Prototype — Kritika
- Created tool schema in structured JSON format for DeepSeek function calling
- Built full Temperature Agent with agentic reasoning loop
- Validated mock endpoint response structure

### Card 8: User Interaction Flow Design — Nandini
- Identified common user query patterns for weather and AQI
- Created flowchart showing system query interpretation and tool selection
- Provided guidelines for consistent user experience

### Card 9: Weekly Team Sync & Documentation — All Members
- Held team sync to align on progress and next steps
- Documented meeting notes and decisions
- Reviewed proof of concept results and planned Week 7 tasks

## 📁 Files
| File | Description |
|------|-------------|
| `temp_agent.ipynb` | Full Temperature Agent — Proof of Concept |

## 🤖 Agent Flow
User Query → DeepSeek-R1:7B (Reasoning) → Tool Call → Open-Meteo API → Structured Weather Report
