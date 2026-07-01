# 🛍️ AI Shopping Assistant Telegram Bot

An intelligent Telegram shopping assistant built using **n8n**, **Google Gemini 2.5 Flash**, and **ScraperAPI**.

This workflow allows users to search for products on Amazon India directly through Telegram and receive AI-powered recommendations. It also acts as a personal styling assistant by providing outfit suggestions based on the user's preferences and occasion.

---

## 📌 Overview

The bot combines conversational AI with workflow automation to deliver a seamless shopping experience.

When a user sends a message to the Telegram bot, the workflow analyzes the request using Google Gemini. If the request is product-related, the bot searches Amazon India using ScraperAPI, extracts relevant product information, and returns the top matching products. For styling-related queries, the AI provides personalized fashion recommendations through a conversational interface.

---

## ✨ Features

- 🤖 AI-powered Telegram chatbot
- 🛒 Amazon India product search
- ⭐ Returns top 5 matching products
- 👕 Personalized styling recommendations
- 🧠 Natural language understanding with Google Gemini
- ⚡ Automated workflow built using n8n
- 🌐 Real-time web scraping using ScraperAPI
- 💬 Interactive conversational experience

---

## ⚙️ Workflow

```text
User
   │
   ▼
Telegram Bot
   │
   ▼
Telegram Trigger (n8n)
   │
   ▼
Google Gemini AI Agent
   │
   ├──────────────┐
   │              │
   ▼              ▼
Product Search    Styling Advice
   │              │
   ▼              ▼
ScraperAPI     AI Recommendations
   │
   ▼
Amazon India Results
   │
   ▼
Top 5 Products
   │
   ▼
Telegram Response
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| n8n | Workflow Automation |
| Telegram Bot API | User Interaction |
| Google Gemini 2.5 Flash | AI Agent |
| ScraperAPI | Web Scraping |
| HTTP Request Node | API Communication |
| Amazon India | Product Source |

---

## 📂 Project Structure

```
Telegram-AI-Shopping-Assistant/
│
├── workflow.json
├── README.md
└── screenshots/
    ├── workflow.png
    ├── telegram-demo.png
    └── output-demo.png
```

---

## 🚀 How It Works

### Product Search

Example:

```
Running shoes under ₹3000
```

The AI Agent:

- Understands the user's request
- Generates an Amazon India search URL
- Calls ScraperAPI
- Extracts product details
- Returns the top 5 matching products

Each result includes:

- Product Name
- Price
- Rating
- Product Link

---

### Styling Assistant

Example:

```
How should I style a blue kurti?
```

The assistant asks follow-up questions such as:

- Occasion
- Preferred style
- Color preferences
- Weather

Then provides:

- Outfit combinations
- Footwear suggestions
- Accessories
- Styling tips

---

## 📸 Screenshots

### n8n Workflow

> *(Add workflow screenshot here)*

---

### Telegram Conversation

> *(Add Telegram chatbot screenshot here)*

---

### Sample Output

> *(Add product recommendation screenshot here)*

---

## 💡 Future Improvements

- Flipkart Integration
- Multi-platform shopping support
- Product image previews
- Price comparison across websites
- Wishlist management
- Voice-based product search
- User preference memory
- Personalized shopping recommendations

---

## 🔒 Security

API keys and credentials should never be committed to the repository.

Store all secrets securely using n8n Credentials or environment variables before deploying.

---

## 🎯 Learning Outcomes

Through this project I learned:

- Workflow Automation with n8n
- Building AI Agents
- Telegram Bot Integration
- Prompt Engineering
- HTTP APIs
- Web Scraping
- AI-powered Automation
- End-to-End Workflow Design

---

## 👨‍💻 Author

**Raviteja**

Artificial Intelligence & Machine Learning Student  
PES University, Bengaluru

---

## ⭐ If you found this project interesting, consider giving it a Star!
