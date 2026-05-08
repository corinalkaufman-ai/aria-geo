# ARIA — AI GEO Team Leader

Your AI-powered GEO team member. Runs GBP audits, content strategy, website optimization, and monthly reports for any client.

---

## Deploy to Vercel in 5 steps (no coding required)

### What you need first
- A free account at **vercel.com**
- A free account at **github.com**
- Your **Anthropic API key** from console.anthropic.com

---

### Step 1 — Put the files on GitHub

1. Go to **github.com** and click the **+** button → **New repository**
2. Name it `aria-geo` and click **Create repository**
3. Click **uploading an existing file**
4. Upload ALL files from this folder, keeping the folder structure:
   ```
   package.json
   vite.config.js
   index.html
   src/main.jsx
   src/App.jsx
   ```
5. Click **Commit changes**

---

### Step 2 — Connect to Vercel

1. Go to **vercel.com** and click **Add New Project**
2. Click **Import Git Repository** and select your `aria-geo` repo
3. Vercel will auto-detect it as a Vite project — leave all settings as default
4. **Do NOT click Deploy yet** — go to Step 3 first

---

### Step 3 — Add your API key

Still on the Vercel setup screen:

1. Scroll down to **Environment Variables**
2. Add this exact variable:
   - **Name:** `VITE_ANTHROPIC_API_KEY`
   - **Value:** your Anthropic API key (starts with `sk-ant-...`)
3. Click **Add**

---

### Step 4 — Deploy

1. Click **Deploy**
2. Wait ~60 seconds
3. Vercel gives you a URL like `aria-geo-yourname.vercel.app`

That's it. ARIA is live.

---

### Step 5 — Custom domain (optional)

To use `aria.youragency.com`:

1. In your Vercel project, go to **Settings → Domains**
2. Add your custom domain
3. Follow the DNS instructions (add a CNAME record in your domain registrar)
4. Done in under 10 minutes

---

## Adding team members

Share the URL. Anyone with the link can use ARIA — no login required by default.

To add password protection: in Vercel go to **Settings → Deployment Protection** and enable **Password Protection** (requires Vercel Pro, $20/month).

---

## Plugging in Tier 2 API keys (BrightLocal, DataForSEO, Whitespark)

When you're ready to add enhanced rank tracking and citation data:

1. Go to **Vercel → Settings → Environment Variables**
2. Add `VITE_BRIGHTLOCAL_API_KEY` with your BrightLocal key
3. Redeploy (Vercel does this automatically when you save)

---

## Costs

| Service | Cost |
|---------|------|
| Vercel hosting | Free |
| Anthropic API | ~$0.003 per message (Claude Sonnet) |
| Custom domain | Whatever you pay for your domain |

A typical session with ARIA (10-15 messages including a full audit) costs roughly $0.05-0.15 in API usage.

---

## Updating ARIA

When you want to make changes:

1. Edit the files in your GitHub repo
2. Vercel automatically redeploys within 60 seconds

---

Built with React + Vite + Claude API
