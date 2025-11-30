# 🛍️ Voice-Based E-commerce Agent Hoodies

<div align="center">

![Version](https://img.shields.io/badge/Version-1.0.0-blue)
![Python](https://img.shields.io/badge/Python-3.11-yellow?logo=python)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-F7DF1E?logo=javascript)
![JSON](https://img.shields.io/badge/Storage-JSON-orange?logo=json)
![Realtime](https://img.shields.io/badge/OpenAI-Realtime-412991?logo=openai)
![Voice](https://img.shields.io/badge/TTS-Murf%20Falcon-orange)
![License](https://img.shields.io/badge/License-MIT-green)

**A Voice-Enabled E-commerce Shopping Agent that lets users browse hoodies, filter items, ask for details, and place orders — all through natural voice commands.
Inspired by the Agentic Commerce Protocol (ACP).
Built for the #MurfAIVoiceAgentsChallenge.**

[Features](#-features) • [Project-Structure](#️-project-structure) • [Quick-Start](#-quick-start) • [Demo](#-demo-video) • [Author](#-author)

</div>

---

<img width="1105" height="619" alt="Screenshot 2025-11-30 193210" src="https://github.com/user-attachments/assets/f9678dbc-8e8b-4e44-bb8b-358e5d233234" />

---

## 🛒 Overview

This project is a **voice-controlled E-commerce Assistant** that simulates an ACP-inspired shopping flow.

Your agent can:

✔ Understand shopping intent
✔ Browse hoodie catalog
✔ Filter by size, color, price, category
✔ Add items to cart
✔ Create orders with ACP-like structure
✔ Save orders to JSON with timestamps
✔ Retrieve “What did I just buy?”


https://github.com/user-attachments/assets/aa4ce2da-f2eb-44b3-9d78-07046d990e1a


---

## 🎯 Primary Goal (MVP)

### **Voice Shopping → ACP-Style Order JSON**

### 🧾 **1. Browse a Product Catalog**

The catalog contains:

* Hoodies
* T-shirts
* Accessories
* Shoes
* Color, size, and price attributes

---

### 🎧 **2. Understand Natural Language Shopping Requests**

Examples:

* “Show me black hoodies under ₹1000.”
* “Do you have medium-size hoodies?”
* “I want a blue T-shirt.”

---

### 🛒 **3. Add Items to Cart**

Handles context-aware actions:

* “Buy the second hoodie you mentioned.”
* “Add that one in size L.”
* “Remove the T-shirt.”

---

### 📦 **4. Create ACP-Style Orders**

When the user says *“Place my order”*, the agent:

* Creates a structured order
* Saves to `orders/order_XXX.json`
* Computes total price
* Generates unique order ID
* Stores timestamps

---

## 🚀 Advanced Features

### **📢 Voice Interaction (Murf Falcon)**

Fastest TTS engine for smooth back-and-forth conversation.

---

### **📚 Order History**

Your agent recognizes:

* “What did I just buy?”
* “Show my last order.”
* “Repeat my previous order.”

---

### **🧠 ACP-Inspired Data Models**

Order includes:

* `line_items`
* `total_amount`
* `currency`
* `created_at`
* `status`

---

## ⭐ Features

### ✔ Natural Voice Shopping

Understands flexible inputs:

* “Find hoodies below 800 rupees.”
* “Is the black one available in XL?”
* “Add one more of that.”

---

### ✔ Smart Catalog Filtering

Supports:

* Category
* Color
* Size
* Max price
* Keyword search

---

### ✔ JSON-Powered Storage

Everything stored locally:

* `catalog.json`
* `orders/order_003.json`
* `history.json`

---

### ✔ Realistic ACP Flow (Lite)

Separation of:

* Conversation logic
* Merchant logic
* Data models

---

## 🛠️ Tech Stack

* **Python** — backend agent logic
* **JSON** — catalog + order storage
* **OpenAI Realtime** — voice pipeline
* **Murf Falcon** — STT + TTS
* **Structured Tool Calling**
* **Optional Docker**

---

## 📁 Project Structure

```
/Ecommerce-Voice-Agent
│
├── data/
│   ├── catalog.json
│   ├── history.json
│   └── orders/
│       ├── order_001.json
│       └── order_002.json
│
├── src/
│   ├── agent.py
│   ├── merchant_api.py
│   ├── catalog_service.py
│   ├── order_service.py
│   └── utils/
│
├── logs/
├── requirements.txt
└── README.md
```

---

## ⚙️ Quick Start

### **1. Clone the Repo**

```bash
git clone https://github.com/yourusername/Ecommerce-Voice-Agent
cd Ecommerce-Voice-Agent
```

### **2. Install Dependencies**

```bash
pip install -r requirements.txt
```

### **3. Run the Voice Agent**

```bash
python src/agent.py
```

---

## 🧪 Sample Order JSON

```json
{
  "order_id": "ORDER-2025-001",
  "created_at": "2025-11-29T14:23:00",
  "currency": "INR",
  "line_items": [
    {
      "product_id": "hoodie-002",
      "name": "Black Premium Hoodie",
      "quantity": 1,
      "unit_price": 899
    }
  ],
  "total": 899,
  "status": "CONFIRMED"
}
```

---

## 🎥 Demo Video

📎 https://drive.google.com/file/d/1Rneq2iM6uDwFGaTH2aZeZcfhneiWUePv/view?usp=vids_web

---

## 📌 Future Improvements

* Add UI “Click to Buy” (React)
* ACP-style HTTP endpoints
* Payment simulation
* Real-time stock updates
* Vector search for smarter recommendations

---

## 👨‍💻 Author

**Om Gedam**
GitHub: **@itsomg134**
Email: **[omgedam123098@gmail.com](mailto:omgedam123098@gmail.com)**
Twitter (X): **@omgedam**
LinkedIn: **Om Gedam**
Portfolio: **[https://ogworks.lovable.app](https://ogworks.lovable.app)**
