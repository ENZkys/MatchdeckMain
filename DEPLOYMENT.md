# DEPLOYMENT GUIDE

## 🚀 Quick Start to Production

### Step 1: Install Git (Windows)
```
Download: https://git-scm.com/download/win
Run installer → Accept all defaults → Restart terminal
```

### Step 2: Create GitHub Repository
```
1. Go to https://github.com/new
2. Repository name: matchdeck
3. Description: Profile card sharing platform
4. Public or Private (your choice)
5. Click "Create repository"
```

### Step 3: Push Code to GitHub
```powershell
cd C:\Users\HP\MatchDeck

git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

git init
git add .
git commit -m "Initial commit: MatchDeck project"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/matchdeck.git
git push -u origin main
```

### Step 4: Deploy on Netlify (FREE - Gets You a Domain!)
```
1. Go to https://netlify.com
2. Sign up with GitHub
3. Click "New site from Git"
4. Select your GitHub repo
5. Build settings:
   - Build command: (leave empty)
   - Publish directory: matchdeck/matchdeck-frontend
6. Click "Deploy site"
```

**You'll get a free domain like:** `vibrant-meerkat-a1b2c3.netlify.app`

### Step 5: Custom Domain (Optional)
In Netlify dashboard:
- Site settings → Domain management
- Add your custom domain (requires domain purchase: ~$10/year)

---

## 📝 After Deployment

Update your card creation form to use live API:
- Frontend works immediately ✅
- Cards save to localStorage (works without backend)
- Backend optional for persistent storage

---

## 🎯 Commands Reference

```bash
# View git status
git status

# Make changes and push
git add .
git commit -m "description"
git push

# View commit history
git log --oneline
```

Done! Your site will be live within 1-2 minutes of pushing to GitHub.
