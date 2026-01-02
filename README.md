# HealthWise AI - Local Development

## Quick Start (Offline Testing)

### Option 1: Simple Local Server (No API)

Just open the HTML file or use a simple server:

```bash
# Using Python (if installed)
python3 -m http.server 8000

# Or using Node.js
npx serve .

# Then open: http://localhost:8000
```

**Note**: The API won't work with this method, but you can see the UI.

### Option 2: Full Local Development (With API)

1. **Install dependencies:**
```bash
npm install
```

2. **Set up environment variable:**
Make sure `.env` file exists with:
```
GEMINI_API_KEY=AIzaSyAe9ufBh6xamANbME-ieD3OicjJO3BQE2I
```

3. **Run Netlify Dev (runs both frontend + API locally):**
```bash
npm run dev
# or
netlify dev
```

4. **Open browser:**
```
http://localhost:8888
```

The API will be available at `http://localhost:8888/api/analyze`

### Option 3: Direct File Open

You can also just double-click `index.html` to open it in your browser, but:
- API calls won't work (CORS issues)
- You'll see the UI but can't test the analysis feature

## Testing the API Locally

Once `netlify dev` is running, test with:

```bash
curl -X POST http://localhost:8888/api/analyze \
  -H "Content-Type: application/json" \
  -d '{
    "reportText": "Fasting glucose: 145 mg/dL, Hemoglobin: 11.2 g/dL",
    "age": 28,
    "gender": "F",
    "conditions": ["Gestational Diabetes"]
  }'
```

## Troubleshooting

- **API key error**: Make sure `.env` file exists with `GEMINI_API_KEY`
- **Port already in use**: Change port in `netlify.toml` or kill the process using port 8888
- **Function not found**: Make sure `netlify/functions/analyze.js` exists

