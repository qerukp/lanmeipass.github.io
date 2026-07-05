# lanmeipass.github.io
# 🌊 LanMei Pass - Cross-Border Digital Trade Governance Platform

![Status](https://img.shields.io/badge/Status-Prototype_Demo-blue)
![Tech Stack](https://img.shields.io/badge/Tech-HTML5%20|%20CSS3%20|%20JS-f39f37)
![AI](https://img.shields.io/badge/AI_Engine-DeepSeek-10b981)
![Map](https://img.shields.io/badge/Map-Leaflet.js-199900)

**LanMei Pass** is a one-stop digital governance platform designed to dismantle cross-border trade barriers across the six Lancang-Mekong countries (China, Myanmar, Laos, Thailand, Cambodia, and Vietnam). Powered by a **"Blockchain + AI"** dual-engine architecture, the platform aims to reduce the hidden trade barriers faced by SMEs, such as fragmented documentation, high trust costs, and opaque logistics.

---

## ✨ Core Features

1. 📊 **Dashboard Console**
   - Real-time monitoring of core cross-border trade metrics (YTD tariff savings, average clearance time, supply chain security index).
   - Dynamic updates and briefs on RCEP tariff dividends.

2. 🆔 **Cross-Border Decentralized Identity (DID)**
   - Built on consortium blockchain technology, providing a "One-Time Verification, Six-Nation Recognition" sovereign digital identity framework.
   - Eliminates the need for redundant corporate qualification audits across different national authorities.

3. 📜 **AI Compliance & Document Engine**
   - Automated calculation of RCEP rules of origin (e.g., RVC 40% threshold).
   - Upload trade contracts/invoices to automatically analyze and generate standard compliance documents (e.g., FORM D) required by destination customs.

4. 📍 **Supply Chain Logistics Tracking & Risk Control**
   - Integrated with `Leaflet.js` to visualize the intermodal transport arteries (e.g., Kunming ➔ Mohan ➔ Vientiane ➔ Laem Chabang).
   - AI algorithms predict port congestion 3-7 days in advance and issue route warnings.

5. ⚡ **Parallel Approval Grid**
   - Demonstrates a cross-border collaborative parallel approval workflow, eliminating clearance bottlenecks caused by traditional sequential processing.

6. 🤖 **AI Assistant (Chatbot)**
   - Integrated with the DeepSeek LLM, providing professional answers to queries regarding RCEP tariffs, customs compliance, and platform operations.
   - Supports seamless context switching between English and Chinese.

7. 🌐 **Dynamic i18n (Multilingual Support)**
   - One-click toggle between English and Chinese (Simplified), covering navigation menus, reports, and AI system prompts.

---

## 🛠️ Tech Stack

This project is currently built on a **Vanilla Web** architecture. No complex build tools (like Webpack or Vite) are required, making it ready to run out of the box:
- **Core:** HTML5, CSS3, Vanilla JavaScript (ES6+)
- **Map Rendering:** [Leaflet.js](https://leafletjs.com/) (with CARTO Dark tile layer)
- **AI Integration:** Fetch API (connecting to DeepSeek Cloud API)
- **Cryptography:** [CryptoJS](https://cryptojs.gitbook.io/) (Reserved for complex WebSocket authentication, e.g., iFlytek Spark)

---

## 🚀 Local Setup & Configuration

### 1. Clone/Download the Repository
Download the source code to your local machine and ensure the `index.html` file is present.

### 2. Configure the LLM API Key
Open `index.html`, scroll to the `<script>` section at the bottom, and locate the `CONFIG` object:
```javascript
const CONFIG = {
    deepseek: {
        apiKey: "sk-YOUR_REAL_API_KEY_HERE", // 👈 Replace with your DeepSeek API Key
        apiUrl: "[https://api.deepseek.com/chat/completions](https://api.deepseek.com/chat/completions)"
    },
    // ... other reserved configs
};
