# Netlify Deployment Guide for Your Portfolio

## Quick Deploy Steps

### Method 1: Drag and Drop (Easiest - No Git Required)

1. **Prepare Your Files**
   - Make sure all files are in the portfolio folder
   - Main files needed: `index.html`, `styles.css`, images (logo.jpeg, profilepic.jpeg)
   - Video folder: `video/footer.mp4`

2. **Go to Netlify**
   - Visit: https://app.netlify.com
   - Sign up/Login (free account)

3. **Deploy**
   - Drag your entire folder `portfolio latest` onto Netlify's deploy area
   - Wait for deployment (takes 1-2 minutes)
   - Your site will be live with a random URL like `random-name-123.netlify.app`

4. **Get Custom Domain** (Optional)
   - Click on your site
   - Go to "Domain settings"
   - Add custom domain or use the free Netlify subdomain

### Method 2: Git Deployment (Recommended - Auto Updates)

1. **Create GitHub Repository**
   ```bash
   # In your portfolio folder, run:
   git init
   git add .
   git commit -m "Initial portfolio deployment"
   ```

2. **Push to GitHub**
   - Create a new repository on GitHub.com
   - Push your code:
   ```bash
   git remote add origin https://github.com/yourusername/portfolio.git
   git push -u origin main
   ```

3. **Connect to Netlify**
   - Go to Netlify → "Add new site" → "Import an existing project"
   - Choose GitHub → Select your repository
   - Netlify will auto-deploy
   - **Auto-deploy**: Every time you push to GitHub, Netlify updates your site!

## Making Changes After Deployment

### If Using Git (Method 2 - Best):
1. Edit files locally
2. Commit changes:
   ```bash
   git add .
   git commit -m "Updated portfolio"
   git push
   ```
3. Netlify automatically deploys (takes 1-2 minutes)
4. Done! Your site is updated

### If Using Drag & Drop (Method 1):
1. Edit files locally
2. Drag and drop the folder again on Netlify
3. Or use Netlify's file editor (limited)
4. Or use their CLI: `netlify deploy`

## File Structure for Netlify

Your folder should have:
```
portfolio latest/
├── index.html          (main file)
├── styles.css          (styles)
├── logo.jpeg           (SSEV logo)
├── profilepic.jpeg     (profile photo)
└── video/
    └── footer.mp4      (skills section video)
```

## Important Settings in Netlify

### Build Settings (if needed):
- **Build command**: Leave empty (static site)
- **Publish directory**: `./` (root folder)

### Environment Variables:
- Not needed for this portfolio (all static files)

## Custom Domain Setup

1. In Netlify Dashboard → Your Site → Domain settings
2. Click "Add custom domain"
3. Enter your domain (e.g., `praneethsai.com`)
4. Follow DNS configuration instructions
5. Netlify provides free SSL certificate automatically!

## Tips

✅ **Always test locally** before deploying  
✅ **Keep backups** of your files  
✅ **Use Git** for easy updates  
✅ **Check console** for any errors after deployment  
✅ **Use Netlify's preview** to test before going live  

## Troubleshooting

**Images not loading?**
- Check file paths (case-sensitive!)
- Ensure images are in the folder

**Video not playing?**
- Check `video/footer.mp4` path
- Video file size might be large (Netlify has limits)

**Styles not applying?**
- Clear browser cache (Ctrl+Shift+R)
- Check CSS file path in index.html

## Netlify Free Tier Includes:
- ✅ Unlimited bandwidth
- ✅ Free SSL certificate
- ✅ Custom domains
- ✅ Form handling (you're using EmailJS, so not needed)
- ✅ Continuous deployment from Git

---

**Your site will be live at:** `your-site-name.netlify.app`


