# Deployment Guide - GitHub Pages Staging

## Quick Setup Steps

### Step 1: Create Repository on GitHub
1. Go to https://github.com/new
2. Repository name: `Betstudio-Dashboard`
3. Make it **Public** (required for free GitHub Pages)
4. **DO NOT** initialize with README, .gitignore, or license
5. Click "Create repository"

### Step 2: Push Your Code
Run these commands in your terminal:

```bash
# Verify your remote (should show the GitHub URL)
git remote -v

# If remote is correct, push:
git push -u origin main
```

If the repository doesn't exist yet, GitHub will show you the commands to run after creating it.

### Step 3: Enable GitHub Pages
1. Go to your repository on GitHub: `https://github.com/Garimadasila4/Betstudio-Dashboard`
2. Click **Settings** tab
3. Scroll down to **Pages** (in left sidebar)
4. Under "Source", select **GitHub Actions**
5. Save

### Step 4: Deploy
The GitHub Actions workflow will automatically:
- Deploy on every push to `main` branch
- Create a staging site at: `https://garimadasila4.github.io/Betstudio-Dashboard/`

### Step 5: View Your Staging Site
After the workflow completes (takes 1-2 minutes):
- Go to **Actions** tab in your repository
- Click on the latest workflow run
- Wait for "Deploy to GitHub Pages" to complete
- Visit: `https://garimadasila4.github.io/Betstudio-Dashboard/`

## Manual Push (If Remote Doesn't Work)

If you need to set up the remote manually:

```bash
# Remove old remote
git remote remove origin

# Add correct remote (replace with your actual GitHub username if different)
git remote add origin https://github.com/Garimadasila4/Betstudio-Dashboard.git

# Push
git push -u origin main
```

## Troubleshooting

### Repository Not Found Error
- Make sure you created the repository on GitHub first
- Verify your GitHub username is correct
- Check repository name matches exactly

### Pages Not Showing
- Make sure repository is **Public**
- Verify GitHub Actions workflow ran successfully
- Check Settings → Pages → Source is set to "GitHub Actions"
- Wait 2-3 minutes for deployment to complete
