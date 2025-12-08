# 📋 Pre-Deployment Checklist

Before deploying your portfolio website, make sure you've completed these steps:

## ✅ Content Updates

- [x] **Personal Information**
  - [x] Name updated throughout the site
  - [x] Email address (mr.adiras@gmail.com)
  - [x] Current job title and company
  - [x] Bio/tagline updated

- [x] **Social Links**
  - [x] GitHub: https://github.com/OxAdiras
  - [x] LinkedIn: https://linkedin.com/in/adirassahu
  - [x] Email link working
  - [x] Resume link pointing to Adiras_Resume.pdf

- [x] **Professional Content**
  - [x] Work experience section updated
  - [x] Education details correct
  - [x] Projects showcased
  - [x] Skills and technologies listed
  - [x] Achievements included

## 📝 Files to Review

- [ ] **index.html** - Check all content is yours
- [ ] **resume/Adiras_Resume.pdf** - Latest version uploaded
- [ ] **README.md** - Instructions are clear
- [ ] **.gitignore** - Unnecessary files excluded

## 🖼️ Images to Update (Optional but Recommended)

The website currently uses your friend's company logos. You may want to add/update:

- [ ] `img/organization/nomura.gif` - Already exists (good!)
- [ ] `img/organization/sgsits_logo.png` - Add SGSITS logo
- [ ] `img/organization/coding_platforms.png` - Add coding platform logos
- [ ] `img/vp.png` - Consider replacing with your own profile/brand image
- [ ] `img/emoji/technologist.png` - Favicon (currently generic, can personalize)

### How to Add Images:
1. Find the logo/image online or create your own
2. Save it in the appropriate `img/organization/` folder
3. Update the `<img src="...">` path in `index.html` if needed

## 🧪 Local Testing

Before deploying, test locally:

- [ ] Open `index.html` in a web browser
- [ ] Check all sections display correctly
- [ ] Click all links to verify they work
- [ ] Test dark mode toggle
- [ ] Test on mobile view (browser dev tools)
- [ ] Check resume PDF opens correctly

### Test Responsiveness:
- [ ] Desktop view (1920px)
- [ ] Laptop view (1366px)
- [ ] Tablet view (768px)
- [ ] Mobile view (375px)

## 🔍 Content Accuracy

Double-check these details:

- [ ] All dates are correct (work experience, education)
- [ ] Company names spelled correctly
- [ ] Email address has no typos
- [ ] GitHub username is correct (OxAdiras)
- [ ] LinkedIn URL is correct (adirassahu)
- [ ] Project descriptions are accurate
- [ ] Technical skills list is current

## 📱 Contact Information

Verify all contact methods work:

- [ ] Email link opens mail client: mr.adiras@gmail.com
- [ ] LinkedIn link goes to correct profile
- [ ] GitHub link goes to correct profile
- [ ] Resume PDF downloads correctly

## 🎨 Customization (Optional)

Consider personalizing:

- [ ] Color scheme (edit `css/main.css`)
- [ ] Greeting messages (currently multilingual)
- [ ] Section order
- [ ] Add a blog section
- [ ] Add more projects
- [ ] Add skills section with visual indicators

## 🚀 Deployment Preparation

Before pushing to GitHub:

- [ ] Remove any test/dummy content
- [ ] Delete unnecessary files from `old/` folder (or remove folder)
- [ ] Ensure no sensitive information in code
- [ ] Check file sizes (GitHub has 100MB file limit)
- [ ] Verify all paths are relative (not absolute local paths)

## 📊 GitHub Repository Setup

Prepare for GitHub:

- [ ] Choose repository name
  - Recommended: `OxAdiras.github.io` (for username.github.io URL)
  - Or: `portfolio`, `personal-website`, etc.
- [ ] Repository will be Public (required for free GitHub Pages)
- [ ] .gitignore file is in place
- [ ] README.md is informative

## 🌐 Domain Planning

Decide on your domain strategy:

- [ ] **Option 1**: Use GitHub Pages default
  - URL: `https://oxadiras.github.io`
  - No additional setup needed
  - Ready immediately

- [ ] **Option 2**: Add .is-a.dev subdomain
  - URL: `https://adiras.is-a.dev` (or your choice)
  - Requires PR to is-a-dev repository
  - Takes 1-3 days for approval

- [ ] **Option 3**: Use your own custom domain
  - URL: `https://yourdomain.com`
  - Requires purchasing domain
  - Update DNS settings

## ✨ Final Checks

- [ ] All TODO comments removed from code
- [ ] Console has no errors (check browser dev tools)
- [ ] All images load correctly
- [ ] Typography is readable
- [ ] Links are visible and distinguishable
- [ ] Footer displays current year (automatic via JavaScript)

## 📋 Deployment Steps

When ready, follow these steps:

1. [ ] Run `git init` in project directory
2. [ ] Run `git add .`
3. [ ] Run `git commit -m "Initial commit"`
4. [ ] Create GitHub repository
5. [ ] Add remote: `git remote add origin <URL>`
6. [ ] Push: `git push -u origin main`
7. [ ] Enable GitHub Pages in repository settings
8. [ ] Wait 2-3 minutes for deployment
9. [ ] Visit your site!

## 🎯 Post-Deployment

After going live:

- [ ] Test live site on multiple devices
- [ ] Share link with friends for feedback
- [ ] Update LinkedIn with portfolio link
- [ ] Update GitHub profile with website link
- [ ] Consider adding Google Analytics (optional)
- [ ] Set up custom domain if desired

## 📝 Ongoing Maintenance

Remember to:

- [ ] Update resume periodically
- [ ] Add new projects as you complete them
- [ ] Keep work experience current
- [ ] Update skills as you learn new technologies
- [ ] Fix any broken links
- [ ] Respond to any feedback

## 🆘 Need Help?

If you encounter issues:

1. Check the `DEPLOYMENT.md` guide
2. Review `README.md` instructions
3. Search GitHub Pages documentation
4. Check is-a-dev repository issues
5. Reach out for help

---

## ⚡ Quick Start (If Everything Above is Done)

```powershell
# Navigate to project directory
cd "d:\Projects\personalWebsite\adiras_personal"

# Initialize and push to GitHub
git init
git add .
git commit -m "Initial commit: Adiras Sahu Portfolio"
git remote add origin https://github.com/OxAdiras/OxAdiras.github.io.git
git branch -M main
git push -u origin main

# Then: Enable GitHub Pages in repository Settings → Pages
```

---

**Status**: Ready to deploy! 🚀

**Next Action**: Follow the deployment steps above or refer to `DEPLOYMENT.md`

Good luck with your portfolio launch! 🎉
