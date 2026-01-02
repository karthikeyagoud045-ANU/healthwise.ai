# HealthWise AI - Setup Instructions

## API Key Configuration

### For Local Development:
1. Create a `.env` file in the root directory
2. Add this line:
```
GEMINI_API_KEY=AIzaSyAe9ufBh6xamANbME-ieD3OicjJO3BQE2I
```

### For Netlify Deployment:
1. Go to your Netlify site dashboard
2. Navigate to **Site settings** → **Environment variables**
3. Click **Add variable**
4. Key: `GEMINI_API_KEY`
5. Value: `AIzaSyAe9ufBh6xamANbME-ieD3OicjJO3BQE2I`
6. Click **Save**
7. **Redeploy** your site (go to Deploys → Trigger deploy)

## Local Development

```bash
npm install
netlify dev
```

The site will be available at `http://localhost:8888`

## Testing the API

```bash
curl -X POST http://localhost:8888/api/analyze \
  -H "Content-Type: application/json" \
  -d '{"reportText":"Fasting glucose 145 mg/dL, Hb 11.2 g/dL","age":28,"gender":"F","conditions":["Gestational Diabetes"]}'
```

## Deployment Checklist

- [ ] API key added to Netlify environment variables
- [ ] Site redeployed after adding API key
- [ ] Function logs checked in Netlify dashboard
- [ ] Test API endpoint works

