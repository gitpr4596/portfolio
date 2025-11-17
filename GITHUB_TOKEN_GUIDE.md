# Complete Guide: Getting Repository URL & Creating Personal Access Token

## Part 1: Getting Your Repository URL

### Step 1: Go to Your Repository
1. **Go to [github.com](https://github.com)** and sign in
2. **Click on your profile picture** (top right)
3. **Click "Your repositories"** (or go directly to: `https://github.com/gitpr4596?tab=repositories`)
4. **Click on your "portfolio" repository**

### Step 2: Copy the Repository URL
1. **On your repository page**, look for a green button that says **"Code"** (usually on the right side, near the top)
2. **Click the "Code" button**
3. **A dropdown menu will appear** with three tabs: HTTPS, SSH, and GitHub CLI
4. **Make sure "HTTPS" tab is selected** (it should be by default)
5. **You'll see a URL** that looks like:
   ```
   https://github.com/gitpr4596/portfolio.git
   ```
6. **Click the copy icon** (📋) next to the URL, or select the URL and copy it (Cmd+C on Mac, Ctrl+C on Windows)

**✅ You now have your repository URL!** Save it somewhere - you'll need it for the `git remote add origin` command.

---

## Part 2: Creating a Personal Access Token

GitHub requires a Personal Access Token instead of your password for security. Here's how to create one:

### Step 1: Go to GitHub Settings
1. **Go to [github.com](https://github.com)** and sign in
2. **Click your profile picture** (top right corner)
3. **Click "Settings"** from the dropdown menu
   - Or go directly to: `https://github.com/settings/profile`

### Step 2: Navigate to Developer Settings
1. **Scroll down** on the left sidebar
2. **Click "Developer settings"** (at the bottom of the left menu)
   - Or go directly to: `https://github.com/settings/apps`

### Step 3: Access Personal Access Tokens
1. **In the left sidebar**, click **"Personal access tokens"**
2. **Click "Tokens (classic)"** (not "Fine-grained tokens")
   - Or go directly to: `https://github.com/settings/tokens`

### Step 4: Generate New Token
1. **Click the button** that says **"Generate new token"**
2. **Click "Generate new token (classic)"** from the dropdown
   - You might see a warning about classic tokens - that's okay, click "Generate new token (classic)" anyway

### Step 5: Configure Your Token
Fill in the form:

1. **Note** (required):
   - Type: `Portfolio Upload` or `Git Push Token` or `Portfolio Repository Access`
   - This is just a label to remember what this token is for

2. **Expiration**:
   - Choose: **90 days** (recommended for first time)
   - Or **Custom** if you want a different duration
   - Or **No expiration** (less secure, but convenient)

3. **Select scopes** (permissions):
   - **✅ Check the box next to "repo"** (this gives full repository access)
     - This will automatically check all sub-options:
       - repo:status
       - repo_deployment
       - public_repo
       - repo:invite
       - security_events
   - **That's all you need!** Don't check anything else unless you specifically need it

4. **Scroll down** and click the green **"Generate token"** button

### Step 6: Copy Your Token
⚠️ **IMPORTANT: Copy the token immediately!**

1. **GitHub will show you a token** that looks like:
   ```
   ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
   ```
   (It starts with `ghp_` followed by a long string)

2. **Click the copy icon** (📋) or select and copy the entire token
   - **⚠️ WARNING:** You won't be able to see this token again after you leave this page!
   - **Save it somewhere safe** (password manager, notes app, etc.)

3. **You're done!** You can close this page now.

---

## Part 3: Using the Token

### When Pushing to GitHub

When you run `git push` and GitHub asks for credentials:

1. **Username:** Enter your GitHub username (`gitpr4596`)

2. **Password:** 
   - **DO NOT** enter your GitHub account password
   - **Instead**, paste the Personal Access Token you just created
   - It will look like: `ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx`

3. **Press Enter**

**Note:** Some systems might cache your credentials, so you might not need to enter it every time.

---

## Part 4: Complete Setup Commands

Now that you have both the URL and token, here are the complete commands:

```bash
# 1. Navigate to your project
cd "/Users/mac1ssev/Downloads/portfolio latest"

# 2. Initialize Git (if not done already)
git init

# 3. Add all files
git add .

# 4. Commit
git commit -m "Initial commit: Portfolio website"

# 5. Add remote (USE YOUR ACTUAL URL)
git remote add origin https://github.com/gitpr4596/portfolio.git

# 6. Push to GitHub
git branch -M main
git push -u origin main
```

**When prompted:**
- **Username:** `gitpr4596`
- **Password:** `ghp_your_token_here` (paste your Personal Access Token)

---

## 🔒 Security Tips

1. **Don't share your token** publicly
2. **Don't commit tokens** to your repository
3. **Revoke old tokens** if you think they're compromised:
   - Go to: `https://github.com/settings/tokens`
   - Click the token → Click "Delete"
4. **Use different tokens** for different purposes
5. **Set expiration dates** for better security

---

## ❓ Troubleshooting

### "Authentication failed" or "Invalid credentials"
- **Solution:** Make sure you're using the Personal Access Token (starts with `ghp_`), NOT your GitHub password
- **Solution:** Check if the token has expired
- **Solution:** Make sure you checked the "repo" scope when creating the token

### "Token not found" or "Token expired"
- **Solution:** Create a new token following the steps above

### "Permission denied"
- **Solution:** Make sure the token has "repo" scope checked
- **Solution:** Verify your username is correct

### Token not working after some time
- **Solution:** Check if the token expired (if you set an expiration date)
- **Solution:** Create a new token

---

## 📝 Quick Reference

**Repository URL:**
```
https://github.com/gitpr4596/portfolio.git
```

**Token Location:**
```
GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
```

**Required Scope:**
```
✅ repo (full repository access)
```

**Token Format:**
```
ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

---

## ✅ Checklist

- [ ] Repository URL copied
- [ ] Personal Access Token created
- [ ] Token saved securely
- [ ] Token has "repo" scope
- [ ] Ready to push to GitHub!

---

**Need help?** Check GitHub's official guide: [Creating a personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)

