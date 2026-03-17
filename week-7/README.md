# Week 7 — Tool Agent Development & Data Integration

> **Course:** CPS698 Capstone Project
> **Team 4:** Kritika Gupta | Rohit Manohar Saggam | Nandini Devi Poreddy
> **Mentor:** Dr. Razi Iqbal | **Instructor:** Dr. Michael Johnson

## 📌 Overview
Week 7 focused on building the core tool agents for real-time data retrieval, integrating weather and AQI data sources, and implementing intent classification to route user queries to the correct agent.

## ✅ Completed Cards

### Card 1: Weather Tool Agent — Kritika
- Built get_weather() function using Open-Meteo Forecast API
- Extracts temperature, feels-like, humidity, wind speed, and conditions
- Converts temperature to both Celsius and Fahrenheit
- Returns structured JSON output for the reasoning agent

### Card 2: AQI Tool Agent — Rohit
- Built get_aqi() function using Open-Meteo Air Quality API
- Retrieves PM2.5, PM10, NO2, O3, and CO pollutant levels
- Computes AQI category (Good to Hazardous) based on PM2.5 thresholds
- Implemented fallback logic for cities with limited monitoring data

### Card 3: Dynamic Location-Based Retrieval — Nandini
- Built get_coordinates() using Open-Meteo Geocoding API
- Converts city names to standardized latitude/longitude coordinates
- Handles multiple city queries and validates city names
- Returns clear error messages for invalid inputs

### Card 4: Unified Data Integration Layer — Rohit
- Built get_combined_data() merging weather and AQI outputs
- Returns single consistent JSON with both data sources
- Handles partial failures gracefully
- Includes data_available flags for downstream processing

### Card 5: Intent Classification Module — Kritika
- Defined query categories: weather_only, aqi_only, combined, comparison
- Built keyword-based classifier with weather and AQI keyword dictionaries
- Validated classification accuracy across 6 different query types
- Integrated into pipeline for automatic tool routing

## 📁 Files
| File | Description |
|------|-------------|
| `week7_agents.ipynb` | All 5 modules + full pipeline test |

## 🔄 Pipeline Flow
User Query → Intent Classification → Location Retrieval → Tool Agent Selection → Structured JSON Output

## 🧪 Test Results
- Location Retrieval: Valid and invalid cities tested — Pass
- Weather Agent: New York, London, Tokyo — Pass
- AQI Agent: Delhi, Paris, Sydney — Pass
- Data Integration: Chicago combined query — Pass
- Intent Classification: 6 queries — All classified correctly
- Full Pipeline: 3 end-to-end queries — Pass
