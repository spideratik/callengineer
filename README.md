# Call Engineer — website

Static single-page site. No build step required.

## Deploy to Vercel

### Option A — Vercel dashboard (no CLI, no Git needed)
1. Go to https://vercel.com and log in (or sign up free).
2. Click **Add New → Project**.
3. Choose **"Deploy without Git"** / drag-and-drop, and drop this folder
   (containing `index.html` and `vercel.json`) onto the upload area.
4. Click **Deploy**. Vercel gives you a live URL in under a minute.

### Option B — Vercel CLI
```bash
npm i -g vercel     # one-time install
cd call-engineer    # this folder
vercel               # follow the prompts, choose defaults
vercel --prod        # ship it to your production URL
```

### Option C — GitHub + Vercel (best if you'll keep editing the site)
1. Push this folder to a new GitHub repo.
2. On vercel.com: **Add New → Project → Import Git Repository**, pick the repo.
3. Framework preset: choose **Other** (it's plain HTML, no framework).
4. Deploy. Every future push to the repo auto-deploys.

## Custom domain
After the first deploy, go to your project on vercel.com → **Settings → Domains**
and add your own domain (e.g. `callengineer.com.bd`). Vercel gives you the
DNS records to add at your domain registrar.

## Adding images later
Put image files in an `/images` folder next to `index.html` and reference
them as `images/filename.jpg` in the HTML — see the note in chat for exact
placement.
