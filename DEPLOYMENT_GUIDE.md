# Deployment Guide for praneethsai.com

## Quick Deployment Options

### Option 1: GitHub Pages (Free & Easy)

1. **Create GitHub Repository:**
   - Go to https://github.com/new
   - Create a repository (e.g., "portfolio")
   - Make it public (required for free GitHub Pages)

2. **Upload Files:**
   ```bash
   cd "/Users/mac1ssev/Downloads/portfolio latest"
   git init
   git add .
   git commit -m "Initial portfolio commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/portfolio.git
   git push -u origin main
   ```

3. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Source: Deploy from branch → main branch
   - Your site will be at: `https://YOUR_USERNAME.github.io/portfolio`

4. **Buy Domain & Connect:**
   - Buy `praneethsai.com` from Namecheap, GoDaddy, or Google Domains
   - Add `CNAME` file in repository root with content: `praneethsai.com`
   - Configure DNS:
     - Add A record: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
     - OR add CNAME: `YOUR_USERNAME.github.io`

### Option 2: Netlify (Free & Very Easy)

1. **Sign up at:** https://www.netlify.com

2. **Deploy:**
   - Drag and drop your folder to Netlify dashboard
   - OR connect GitHub repository

3. **Custom Domain:**
   - Go to Site settings → Domain management
   - Add custom domain: `praneethsai.com`
   - Configure DNS as shown in Netlify dashboard

### Option 3: Vercel (Free & Easy)

1. **Sign up at:** https://vercel.com

2. **Install Vercel CLI:**
   ```bash
   npm i -g vercel
   ```

3. **Deploy:**
   ```bash
   cd "/Users/mac1ssev/Downloads/portfolio latest"
   vercel
   ```

4. **Add Domain:**
   - Go to project settings → Domains
   - Add `praneethsai.com`
   - Follow DNS configuration instructions

## Domain Purchase

Recommended domain registrars:
- **Namecheap** (https://www.namecheap.com) - ~$10-15/year
- **Google Domains** (https://domains.google) - ~$12/year
- **GoDaddy** (https://www.godaddy.com) - ~$12-15/year

## Important Notes

1. **File Paths:** Make sure all file paths in your HTML/CSS are relative (use `video/footer.mp4` not `/video/footer.mp4`)

2. **HTTPS:** All hosting options above provide free SSL/HTTPS certificates

3. **Video File:** Ensure `video/footer.mp4` is uploaded and accessible

## Recommended: Netlify (Easiest)

For fastest deployment:
1. Sign up at netlify.com
2. Drag folder to deploy
3. Buy domain from Namecheap
4. Add domain in Netlify settings
5. Configure DNS (takes 24-48 hours)

Your site will be live at **praneethsai.com**!


