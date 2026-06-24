# SmileCare Family Dentistry — AI Patient Assistant

A live demo of an AI-powered patient inquiry and appointment booking system built for dental clinics.

## 🔗 Live Demo

[View Live Demo](https://smilecare-demo.vercel.app)

---

## What This Does

- Answers common dental clinic questions 24/7
- Collects patient intake information (name, phone, email, treatment, preferred date)
- Saves appointment requests automatically to Google Sheets
- Works on desktop and mobile

---

## Tech Stack

| Layer | Tool |
|---|---|
| Frontend | HTML, CSS, JavaScript (single file) |
| Workflow Automation | n8n (self-hosted on Railway) |
| AI Model | Google Gemini 2.5 Flash Lite |
| Lead Storage | Google Sheets |
| Hosting | Vercel |

---

## How It Works

```
Patient types message
        ↓
Frontend sends conversation history to n8n webhook
        ↓
n8n passes it to Gemini AI
        ↓
Gemini responds as SmileCare assistant
        ↓
If booking complete → saves lead to Google Sheets
        ↓
Patient sees response in chat widget
```

---

## Features

- Multi-turn conversation memory
- Handles 20+ real-world patient scenarios including typos, off-topic questions, and rude messages
- Emergency detection — routes urgent cases to clinic phone number
- Graceful fallbacks for empty or unclear input
- Typing indicator and smooth animations
- Mobile responsive

---

## Built By

**Zain** — BS Software Engineering, University of Agriculture Faisalabad  
Freelance AI Automation Developer  


