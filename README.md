# Ben Pitkow — Portfolio Site

## Project Structure

```
/
├── index.html        ← Your portfolio (edit content here)
├── vercel.json       ← Vercel deployment config
├── api/
│   └── chat.js       ← Serverless proxy for chatbot API
└── README.md
```

## Deploying to Vercel (free)

### 1. Push this folder to GitHub
- Create a new repo on github.com (e.g. `ben-pitkow-site`)
- Upload all files in this folder to that repo

### 2. Connect to Vercel
- Go to vercel.com and sign up with your GitHub account
- Click **"Add New Project"**
- Select your GitHub repo
- Click **Deploy** — Vercel auto-detects the config

### 3. Add your Anthropic API key
- In Vercel, go to your project → **Settings → Environment Variables**
- Add a new variable:
  - **Name:** `ANTHROPIC_API_KEY`
  - **Value:** your API key (from console.anthropic.com)
- Click **Save**, then go to **Deployments** and click **Redeploy**

### 4. Your site is live
Vercel gives you a URL like `ben-pitkow-site.vercel.app` immediately.

### 5. Custom domain (optional)
- Buy a domain (e.g. `benpitkow.com`) from Namecheap or Google Domains
- In Vercel: **Settings → Domains → Add Domain**
- Follow Vercel's DNS instructions — takes about 5 minutes

## Getting an Anthropic API Key
1. Go to console.anthropic.com
2. Sign up / log in
3. Go to **API Keys** → **Create Key**
4. Copy the key and paste it into Vercel as shown above

The free tier includes enough credits to handle a portfolio site's worth of chatbot traffic.
