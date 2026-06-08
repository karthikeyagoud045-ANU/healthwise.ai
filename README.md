# 🏥 HealthWise AI

<div align="center">

AI-powered **medical report analysis** tool — upload lab reports and get instant, intelligent health insights powered by Google Gemini.

![Gemini](https://img.shields.io/badge/Gemini-AI-blue)
![Netlify](https://img.shields.io/badge/Netlify-Deployed-brightgreen)
![License](https://img.shields.io/badge/License-MIT-green)

</div>

---

## ✨ Features

- **Medical Report Analysis** — Paste or upload lab report text
- **PDF Support** — Extract text from PDF reports using PDF.js
- **Personalized Insights** — Considers age, gender, and existing conditions
- **AI-Powered** — Google Gemini API for medical analysis
- **Clean UI** — Modern, responsive interface with Inter font

---

## 🛠 Tech Stack

| Technology | Purpose |
|---|---|
| **HTML/CSS/JS** | Single-page application |
| **Google Gemini AI** | Medical report analysis |
| **PDF.js** | PDF text extraction |
| **Netlify Functions** | Serverless API (`/api/analyze`) |
| **Netlify** | Hosting + deployment |

---

## 🚀 Quick Start

### Option 1: Simple Static (UI only, no API)

```bash
# Using Python
python3 -m http.server 8000

# Or using Node.js
npx serve .
```

Open [http://localhost:8000](http://localhost:8000)

### Option 2: Full Local Development (With API)

```bash
npm install
```

Create a `.env` file:

```env
GEMINI_API_KEY=your-g...-key
```

Run:

```bash
npm run dev
# or
netlify dev
```

Open [http://localhost:8888](http://localhost:8888)

### Build & Deploy

Already configured for Netlify. Push to GitHub and connect to Netlify.

---

## 📡 API

### `POST /api/analyze`

Analyzes medical report text with Gemini AI.

**Request:**

```json
{
  "reportText": "Fasting glucose: 145 mg/dL, Hemoglobin: 11.2 g/dL",
  "age": 28,
  "gender": "F",
  "conditions": ["Gestational Diabetes"]
}
```

**Test locally:**

```bash
curl -X POST http://localhost:8888/api/analyze \
  -H "Content-Type: application/json" \
  -d '{"reportText": "Fasting glucose: 145 mg/dL", "age": 28, "gender": "M"}'
```

---

## 📁 Project Structure

```
healthwise.ai/
├── index.html              # Main SPA (UI + Gemini client)
├── netlify.toml            # Netlify config
├── package.json            # Dependencies
├── deno.lock               # Deno lock file
├── SETUP.md                # Detailed setup guide
├── healthwise-prompts.md   # AI prompt templates
└── README.md
```

---

## 🔧 Environment Variables

| Variable | Description | Required |
|---|---|---|
| `GEMINI_API_KEY` | Google Gemini API key | Yes (for API) |

---

