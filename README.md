---
title: Threat Signal — Global Intelligence Network
emoji: 🌍
colorFrom: red
colorTo: gray
sdk: static
pinned: true
license: mit
short_description: AI-powered global threat intelligence with 3D globe and voice agent
tags:
  - threat-intelligence
  - ai-agents
  - crewai
  - llama3
  - amd
  - hackathon
  - security
  - geopolitical
  - voice
  - three.js
---

# 🌐 THREAT SIGNAL — Global Intelligence Network

> **AMD Developer Hackathon 2025 · Track 1: AI Agents**
> Built with Llama 3 on AMD Instinct MI300X · CrewAI · Three.js · Web Speech API

---

## What is Threat Signal?

**Threat Signal** is an AI-powered global threat intelligence platform. Type or speak any city on Earth — five specialized AI agents instantly scan weather disasters, armed conflict, civil unrest, disease outbreaks, and geopolitical risk — then deliver a structured, color-coded threat brief with safety recommendations.

Think of it as a weather app, but for danger.

---

## ✨ Key Features

- **🌍 3D Rotating Globe** — Live threat markers on a real-time Three.js globe. Red = critical, orange = high, yellow = moderate, green = low
- **🤖 5 AI Agents** — Each agent specializes in one threat category. A Synthesizer agent compiles all findings into a unified intelligence brief
- **🎙️ Voice Agent** — Speak a city name, the system scans and reads the threat report back to you in an authoritative voice
- **📊 Threat Analytics** — Animated threat meters, category cards, and safety recommendations for every location
- **🌐 Any Location** — Works for any city, region, or country on Earth. Powered by real geocoding
- **⚡ Instant Demo** — 6 pre-loaded cities (Gaza, Kyiv, Lagos, Kabul, Mexico City, Tokyo) for immediate demonstration with no latency

---

## 🎬 Demo

**Try these cities instantly:**

| City | Country | Threat Level |
|------|---------|--------------|
| Gaza | Palestine | 🔴 CRITICAL |
| Kabul | Afghanistan | 🔴 CRITICAL |
| Kyiv | Ukraine | 🟠 HIGH |
| Lagos | Nigeria | 🟡 MODERATE |
| Mexico City | Mexico | 🟡 MODERATE |
| Tokyo | Japan | 🟢 LOW |

Or **type any city** in the search bar — it geocodes any location on Earth.

---

## 🏗️ Architecture

```
User (voice or text input)
        ↓
   Geocoding Layer (Nominatim / OpenStreetMap)
        ↓
   ┌─────────────────────────────────────────┐
   │           CrewAI Agent Network          │
   │                                         │
   │  Agent 1 — Weather & Natural Disasters  │
   │  Agent 2 — Conflict & Military Activity │
   │  Agent 3 — Civil Unrest & Political     │
   │  Agent 4 — Disease & Health Threats     │
   │  Agent 5 — Threat Synthesizer           │
   └─────────────────────────────────────────┘
        ↓
   Llama 3 on AMD Instinct MI300X
        ↓
   Structured JSON Threat Report
        ↓
   3D Globe + Dashboard + Voice Readout
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| LLM | Llama 3 (8B / 70B) via AMD Developer Cloud |
| GPU | AMD Instinct MI300X |
| Agents | CrewAI multi-agent framework |
| LLM Interface | LangChain (OpenAI-compatible endpoint) |
| 3D Globe | Three.js r128 |
| Voice | Web Speech API (recognition + synthesis) |
| Backend | Python 3.10+ · Node.js 18+ · Express |
| Hosting | Hugging Face Spaces (Static) |
| Data | Open-Meteo · OpenStreetMap · Nominatim |

---

## 🚀 Running Locally

### Frontend only (no AMD credits needed)
```bash
git clone https://github.com/YOUR_USERNAME/threat-signal
cd threat-signal
# Open frontend/index.html in your browser
# Click any demo city — works instantly
```

### Full stack (with AMD Cloud)
```bash
# Install dependencies
pip install -r requirements.txt
npm install

# Configure environment
cp .env.example .env
# Add your AMD Developer Cloud API key and base URL

# Start the API server
npm start

# Open http://localhost:3000
```

### Environment variables
```env
AMD_API_KEY=your-amd-api-key
AMD_BASE_URL=https://your-amd-endpoint/v1
PORT=3000
```

---

## 📁 Project Structure

```
threat-signal/
├── frontend/
│   └── index.html          # Full 3D globe + voice dashboard
├── agents/
│   ├── crew.py             # CrewAI agent definitions + data fetchers
│   └── run.py              # CLI runner (called by API server)
├── api/
│   ├── server.js           # Node.js Express API
│   └── demo_report.json    # Pre-built demo for instant load
├── .env.example
├── requirements.txt
├── package.json
└── README.md
```

---

## 🏆 Hackathon Context

**Event:** AMD Developer Hackathon 2025 on lablab.ai  
**Track:** Track 1 — AI Agents & Agentic Workflows  
**Bonus:** Build in Public + Hugging Face Space  
**Prize pool:** $10,000 + AMD Radeon AI PRO R9700 GPU + HF robot prize  

**Judging criteria this project targets:**
- ✅ **Application of Technology** — 5 specialized CrewAI agents on AMD Instinct MI300X running Llama 3
- ✅ **Originality** — No other team is building threat intelligence with a 3D globe + voice agent
- ✅ **Business Value** — Real use case: governments, NGOs, journalists, corporate risk teams, travelers
- ✅ **Presentation** — Cinematic ops-center UI designed for a memorable demo video

---

## 🌍 Use Cases

- **Travelers** — Check threat levels before booking flights or hotels
- **Journalists** — Rapid situational awareness before field deployment
- **NGOs & Aid Workers** — Pre-deployment safety assessment
- **Corporate Risk Teams** — Executive travel security briefings
- **Governments** — Rapid threat monitoring for diplomatic missions

---

## 📜 License

MIT License — open source, free to use and modify.

---

## 👤 Builder

Built solo by **Mansur** — architecture student, web developer, and AI builder based in Nigeria.  
Combining domain knowledge in urban systems, software engineering, and AI tooling.

- 🌐 Renderit.site — AI architectural rendering platform
- 🛠️ AMD Developer Hackathon 2025 submission

---

*Powered by Llama 3 on AMD Instinct MI300X · CrewAI · Hugging Face · Built for AMD Developer Hackathon 2025*
