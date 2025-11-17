# Fix Git Issues - Quick Commands

## Problem 1: Remote origin already exists

**Fix:** Remove the old remote and add the correct one

```bash
# Remove the old remote
git remote remove origin

# Add the correct remote
git remote add origin https://github.com/gitpr4596/portfolio.git
```

## Problem 2: Files not added to Git

**Fix:** Add all files, then commit

```bash
# Add all files
git add .

# Commit with message
git commit -m "Initial commit: Portfolio website"
```

## Complete Fix - Run These Commands:

```bash
# 1. Remove old remote
git remote remove origin

# 2. Add correct remote
git remote add origin https://github.com/gitpr4596/portfolio.git

# 3. Add all files
git add .

# 4. Commit
git commit -m "Initial commit: Portfolio website"

# 5. Push to GitHub
git push -u origin main
```

When prompted for password, use your Personal Access Token (starts with `ghp_`)

