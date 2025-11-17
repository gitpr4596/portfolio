# Complete Guide: Adding Your Portfolio to GitHub

Follow these steps to upload your portfolio to GitHub and make it live.

## 📋 Prerequisites

- GitHub account (create one at [github.com](https://github.com) if you don't have one)
- Git installed on your computer
  - Check if installed: Open Terminal and type `git --version`
  - If not installed: Download from [git-scm.com](https://git-scm.com/downloads)

---

## 🚀 Step-by-Step Instructions

### Step 1: Create a New Repository on GitHub

1. **Go to GitHub.com** and sign in
2. **Click the "+" icon** in the top right corner
3. **Select "New repository"**
4. **Fill in the details:**
   - **Repository name:** `portfolio` (or `portfolio-website`, `my-portfolio`, etc.)
   - **Description:** "Modern responsive portfolio website - Chekoti Praneeth Sai"
   - **Visibility:** Choose **Public** (so others can see it) or **Private**
   - **⚠️ IMPORTANT:** Do NOT check "Add a README file" (you already have one)
   - **Do NOT** add .gitignore or license (you can add later if needed)
5. **Click "Create repository"**

---

### Step 2: Open Terminal/Command Prompt

**On Mac:**
- Press `Cmd + Space`, type "Terminal", press Enter
- Or go to Applications → Utilities → Terminal

**On Windows:**
- Press `Win + R`, type `cmd`, press Enter
- Or search for "Command Prompt" in Start menu

---

### Step 3: Navigate to Your Project Folder

In Terminal/Command Prompt, type:

```bash
cd "/Users/mac1ssev/Downloads/portfolio latest"
```

**Note:** If you're on Windows, the path will be different. Use:
```bash
cd "C:\Users\YourName\Downloads\portfolio latest"
```

Press Enter. You should now be in your project folder.

---

### Step 4: Initialize Git (First Time Only)

If this is the first time using Git in this folder:

```bash
git init
```

This creates a hidden `.git` folder in your project.

---

### Step 5: Add All Files to Git

```bash
git add .
```

This stages all your files (HTML, CSS, images, etc.) for commit.

**To see what files were added:**
```bash
git status
```

---

### Step 6: Create Your First Commit

```bash
git commit -m "Initial commit: Portfolio website"
```

This saves all your files with a message.

---

### Step 7: Connect to GitHub Repository

**Copy the repository URL from GitHub:**
1. Go to your newly created repository on GitHub
2. Click the green **"Code"** button
3. Copy the HTTPS URL (it looks like: `https://github.com/yourusername/portfolio.git`)

**In Terminal, run:**
```bash
git remote add origin https://github.com/yourusername/portfolio.git
```

**Replace `yourusername` and `portfolio` with your actual GitHub username and repository name!**

---

### Step 8: Push Files to GitHub

```bash
git branch -M main
git push -u origin main
```

**If prompted for credentials:**
- **Username:** Your GitHub username
- **Password:** Use a **Personal Access Token** (not your GitHub password)
  - See "Creating a Personal Access Token" section below

---

### Step 9: Verify Upload

1. **Refresh your GitHub repository page**
2. **You should see all your files:**
   - `index.html`
   - `styles.css`
   - `README.md`
   - Images, etc.

✅ **Success!** Your portfolio is now on GitHub!

---

## 🏷️ Step 10: Add Topics/Tags to Your Repository

1. **Go to your repository on GitHub**
2. **Click the gear icon (⚙️)** next to "About" section
3. **In the "Topics" field**, add these topics (press Enter after each):
   ```
   portfolio
   website
   html5
   css3
   javascript
   responsive-design
   dark-theme
   web-development
   frontend
   personal-website
   interactive
   animations
   netlify
   ```
4. **Click "Save changes"**

---

## 🔑 Creating a Personal Access Token (For Git Push)

GitHub no longer accepts passwords. You need a Personal Access Token:

### Steps:

1. **Go to GitHub.com** → Click your profile picture (top right)
2. **Click "Settings"**
3. **Scroll down** → Click "Developer settings" (left sidebar)
4. **Click "Personal access tokens"** → **"Tokens (classic)"**
5. **Click "Generate new token"** → **"Generate new token (classic)"**
6. **Fill in:**
   - **Note:** "Portfolio Upload"
   - **Expiration:** Choose 90 days or custom
   - **Scopes:** Check **"repo"** (this gives full repository access)
7. **Click "Generate token"**
8. **⚠️ COPY THE TOKEN IMMEDIATELY** (you won't see it again!)
9. **Use this token as your password** when pushing to GitHub

---

## 🔄 Making Updates (After Initial Upload)

Whenever you make changes to your portfolio:

```bash
# Navigate to your project folder
cd "/Users/mac1ssev/Downloads/portfolio latest"

# Add changed files
git add .

# Commit with a message
git commit -m "Updated portfolio: [describe your changes]"

# Push to GitHub
git push
```

**Example commit messages:**
- `"Updated portfolio: Added new project"`
- `"Fixed mobile menu responsiveness"`
- `"Updated contact information"`

---

## 🌐 Next Steps: Deploy to Netlify

Now that your code is on GitHub, you can deploy it to Netlify:

1. **Go to [Netlify.com](https://www.netlify.com)** and sign in
2. **Click "Add new site"** → **"Import an existing project"**
3. **Choose "GitHub"** → Authorize Netlify
4. **Select your repository** (`portfolio`)
5. **Click "Deploy site"**
6. **Your site will be live in 1-2 minutes!**

Every time you push to GitHub, Netlify will automatically update your live site!

---

## ❓ Troubleshooting

### "git: command not found"
- **Solution:** Install Git from [git-scm.com](https://git-scm.com/downloads)

### "fatal: not a git repository"
- **Solution:** Make sure you're in the project folder and run `git init`

### "remote origin already exists"
- **Solution:** Remove and re-add:
  ```bash
  git remote remove origin
  git remote add origin https://github.com/yourusername/portfolio.git
  ```

### "Permission denied" or "Authentication failed"
- **Solution:** Use Personal Access Token instead of password (see Step 10 above)

### "Updates were rejected"
- **Solution:** Pull first, then push:
  ```bash
  git pull origin main --allow-unrelated-histories
  git push
  ```

---

## 📝 Quick Reference Commands

```bash
# Navigate to project
cd "/Users/mac1ssev/Downloads/portfolio latest"

# Check status
git status

# Add all files
git add .

# Commit changes
git commit -m "Your message here"

# Push to GitHub
git push

# View commit history
git log
```

---

## ✅ Checklist

- [ ] GitHub account created
- [ ] Git installed on computer
- [ ] Repository created on GitHub
- [ ] Files committed locally
- [ ] Connected to GitHub remote
- [ ] Files pushed to GitHub
- [ ] Topics added to repository
- [ ] README visible on GitHub
- [ ] Ready to deploy to Netlify!

---

**Need help?** Check GitHub documentation: [docs.github.com](https://docs.github.com)

