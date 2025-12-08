# 🚀 Quick Deployment Guide for GitHub Pages

This is a step-by-step guide to get your portfolio website live on GitHub Pages and .is-a.dev.

## Prerequisites

- Git installed on your computer
- A GitHub account
- This portfolio project ready to deploy

## Part 1: Deploy to GitHub Pages (5 minutes)

### Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com/new)
2. Create a new repository:
   - **Option A (Recommended)**: Name it `YOUR-USERNAME.github.io` (e.g., `OxAdiras.github.io`)
     - Your site will be at: `https://oxadiras.github.io`
   - **Option B**: Use any name (e.g., `portfolio`)
     - Your site will be at: `https://oxadiras.github.io/portfolio`
3. Make it **Public**
4. **Don't** check any initialization options
5. Click "Create repository"

### Step 2: Push Your Code

Open PowerShell in your project directory (`d:\Projects\personalWebsite\adiras_personal`) and run these commands:

```powershell
# Initialize git (if not already initialized)
git init

# Add all files
git add .

# Make first commit
git commit -m "Initial commit: Personal portfolio website"

# Add your GitHub repository as remote
# Replace YOUR-USERNAME and REPO-NAME with your actual values
git remote add origin https://github.com/YOUR-USERNAME/REPO-NAME.git

# Rename branch to main
git branch -M main

# Push to GitHub
git push -u origin main
```

**Example for you:**
```powershell
git init
git add .
git commit -m "Initial commit: Adiras Sahu Portfolio"
git remote add origin https://github.com/OxAdiras/OxAdiras.github.io.git
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Click **Pages** (left sidebar)
4. Under "Build and deployment":
   - **Source**: Deploy from a branch
   - **Branch**: `main`
   - **Folder**: `/ (root)`
5. Click **Save**

**Wait 2-3 minutes**, then your site will be live at `https://your-username.github.io`!

## Part 2: Set Up Custom .is-a.dev Domain (Optional - Takes 1-3 days)

### Step 1: Choose Your Subdomain

Decide on a subdomain name, for example:
- `adiras.is-a.dev`
- `oxadiras.is-a.dev`
- `adirassahu.is-a.dev`

### Step 2: Fork is-a.dev Repository

1. Go to: https://github.com/is-a-dev/register
2. Click the **Fork** button (top right)
3. This creates a copy in your account

### Step 3: Create Domain Configuration

1. In **your forked** repository, click on the `domains` folder
2. Click **Add file** → **Create new file**
3. Name it: `YOUR-SUBDOMAIN.json` (e.g., `adiras.json`)
4. Copy this content (update with your details):

```json
{
  "owner": {
    "username": "OxAdiras",
    "email": "mr.adiras@gmail.com"
  },
  "record": {
    "CNAME": "oxadiras.github.io"
  }
}
```

5. Click **Commit changes**

### Step 4: Create Pull Request

1. Go to the **Pull requests** tab in your forked repo
2. Click **New pull request**
3. Click **Create pull request**
4. Title: `Add adiras.is-a.dev` (or your chosen subdomain)
5. Description: Brief message like "Adding my personal portfolio subdomain"
6. Click **Create pull request**

### Step 5: Wait for Approval

- Maintainers will review your PR (usually 1-3 days)
- They may ask for changes if needed
- Once merged, your domain will be active!

### Step 6: Configure Custom Domain in GitHub

Once your PR is **merged**:

1. Go to your GitHub repository
2. **Settings** → **Pages**
3. Under **Custom domain**, enter: `adiras.is-a.dev` (your subdomain)
4. Click **Save**
5. Wait 24 hours for DNS propagation
6. Once working, check **Enforce HTTPS**

## Part 3: Updating Your Website

Whenever you want to update your website:

```powershell
# Make changes to your files

# Add changes
git add .

# Commit with descriptive message
git commit -m "Update: Added new project"

# Push to GitHub
git push origin main
```

Your site will automatically update within 1-2 minutes!

## Troubleshooting

### Issue: "git: command not found"
**Solution**: Install Git from https://git-scm.com/downloads

### Issue: Authentication failed when pushing
**Solution**: Use GitHub Personal Access Token:
1. Go to GitHub Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Generate new token with `repo` scope
3. Use token as password when prompted

### Issue: Website not showing up
**Solution**: 
- Wait 5 minutes after enabling GitHub Pages
- Check Settings → Pages for any errors
- Make sure `index.html` is in the root directory
- Clear browser cache (Ctrl+Shift+Delete)

### Issue: .is-a.dev domain not working
**Solution**:
- Make sure your PR was merged (check status)
- Wait 24 hours for DNS propagation
- Check DNS with: https://dnschecker.org/
- Ensure CNAME in GitHub Pages matches your subdomain

## Quick Commands Reference

```powershell
# Check git status
git status

# See commit history
git log --oneline

# View remote repositories
git remote -v

# Pull latest changes (if working from multiple computers)
git pull origin main

# Undo last commit (keep changes)
git reset --soft HEAD~1

# See what changed
git diff
```

## Next Steps

1. ✅ Website is live on GitHub Pages
2. ✅ Custom domain configured (optional)
3. 📝 Keep your content updated
4. 🔄 Regular commits to track changes
5. 📊 Monitor traffic with GitHub Insights
6. 🎨 Continue customizing design

## Resources

- **GitHub Pages Docs**: https://docs.github.com/en/pages
- **is-a.dev GitHub**: https://github.com/is-a-dev/register
- **Git Documentation**: https://git-scm.com/doc
- **Test Your Site**: https://validator.w3.org/

---

**Need Help?** Open an issue on GitHub or contact me at mr.adiras@gmail.com

Good luck with your deployment! 🎉
