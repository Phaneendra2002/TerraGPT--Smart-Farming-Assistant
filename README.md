# TerraGPT – LLM-Powered Smart Farming Assistant 🌱🤖

TerraGPT is an intelligent agricultural assistant that combines **structured soil data, live weather APIs, and local Large Language Models (LLMs)** to help farmers make informed decisions about crops, fertilizers, and soil conditions.  

Unlike typical chatbot-style AI tools, TerraGPT uses a **tool-first architecture**, relying on real data sources (databases + APIs) for accuracy and falling back on **LLMs (Mistral-7B, LLaMA-2)** only when necessary. This ensures **reliable, safe, and cost-efficient responses**.  

---

## 🚀 Features
- 🔍 **Tool-First Query Routing** – fetches soil, crop, and weather data before using LLM reasoning.  
- 🌦️ **Real-Time Weather Integration** – uses the OpenWeatherMap API for temperature & humidity data.  
- 🌱 **Soil & Crop Data Lookup** – queries a custom SQLite database built from USDA SSURGO datasets.  
- 🧠 **LLM Fallback** – Mistral-7B and LLaMA-2-7B (via Ollama) handle reasoning-heavy queries.  
- 🛡️ **Safe & Domain-Limited** – filters prompt injections and off-domain queries with security checks.  
- ⚡ **Prompt Engineering** – includes meta prompting, chaining, and caching for accurate, reusable responses.  

---

## 🛠️ Tech Stack
- **Programming:** Python  
- **Frameworks:** Gradio (UI), Ollama (LLM hosting)  
- **Models:** Mistral-7B, LLaMA-2-7B  
- **Databases & APIs:** SQLite, USDA SSURGO data, OpenWeatherMap API, Tavily API  

---

## 📊 Results
- Resolved **70% of farmer queries** directly using structured tools (database + weather API).  
- Used LLMs only for **30% of cases**, improving efficiency and reliability.  
- Prompt caching reduced response latency by **30–40%** during testing.  
- Successfully blocked **100% of prompt injection attempts** during robustness evaluation.  

---
