# Netlify Deployment - Step by Step

## CURRENT STEP: Drag & Drop Deployment

You're on the Netlify "Add your project" page. Follow these steps:

### RIGHT NOW:

1. **Scroll down** to the section that says "...or deploy manually"
2. **Find the dashed box** that says "Drag and drop your project folder here"
3. **Open Finder** (on your Mac)
4. **Navigate to:** `/Users/mac1ssev/Downloads/portfolio latest`
5. **Drag the entire folder** `portfolio latest` onto the dashed box in Netlify
6. **Wait 1-2 minutes** for deployment

### What Happens Next:

- Netlify will process your files
- You'll see a progress bar
- When done, you'll get a success message
- Your site URL will appear (like: `random-name-123.netlify.app`)
- Click the URL to see your live site!

---

## FUTURE UPDATES: Making Changes

### Option A: Quick Update (Drag & Drop Again)
1. Edit your files locally (index.html, styles.css, etc.)
2. Go back to Netlify dashboard
3. Drag and drop the folder again
4. Site updates in 1-2 minutes

### Option B: Connect to GitHub (Auto-Updates) ⭐ RECOMMENDED

**Setup Once:**
1. In Netlify, click "Add new site" → "Import from Git"
2. Choose "GitHub"
3. Authorize Netlify to access GitHub
4. Select/create your repository
5. Click "Deploy site"

**Then for Updates:**
1. Edit files locally
2. Push to GitHub:
   ```bash
   git add .
   git commit -m "Updated portfolio"
   git push
   ```
3. Netlify automatically deploys (1-2 minutes)
4. Done!

---

## Custom Domain (Optional)

1. Click your site in Netlify dashboard
2. Go to "Domain settings"
3. Click "Add custom domain"
4. Enter domain name (e.g., `praneethsai.com`)
5. Follow DNS configuration instructions
6. Free SSL certificate automatically provided!

---

## Quick Checklist After Deployment:

- [ ] Site loads correctly
- [ ] All images display (logo.jpeg, profilepic.jpeg)
- [ ] Video plays in Skills section
- [ ] Navigation works
- [ ] Contact form works
- [ ] Responsive on mobile

---

**Need help?** Check Netlify docs: https://docs.netlify.com


