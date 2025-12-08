# Adiras Sahu - Personal Portfolio Website

Welcome to my personal portfolio website! This site showcases my experience, projects, and achievements as a Software Engineer specializing in Autonomous Multi-Agent Systems, RAG Pipelines, and Scalable Cloud Infrastructure.

## 🚀 About Me

I'm a 2025 Graduate currently working as a Software Engineer at Nomura Services, Mumbai. I specialize in:
- **Autonomous Multi-Agent Systems**
- **RAG Pipelines**
- **Scalable Cloud Infrastructure (AWS/Docker)**
- **ETL Pipelines & Data Warehousing**
- **AI/ML Solutions**

## 🛠️ Technologies Used

This website is built using:
- HTML5
- CSS3 (with custom Apercu font)
- JavaScript (jQuery)
- ScrollReveal.js for animations
- Darkmode.js for dark mode toggle

## 📦 Project Structure

```
.
├── index.html              # Main website file
├── css/
│   └── main.css           # Styling
├── js/
│   ├── main.js            # Custom JavaScript
│   ├── jquery.min.js      # jQuery library
│   └── scrollreveal.min.js # Scroll animations
├── img/
│   ├── emoji/             # Emoji images
│   ├── organization/      # Company/org logos
│   └── social/            # Social media icons
├── font/                  # Custom Apercu fonts
├── resume/
│   └── Adiras_Resume.pdf  # My resume
└── README.md              # This file
```

## 🌐 Hosting on GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and create a new repository
2. Name it: `your-username.github.io` (e.g., `OxAdiras.github.io`)
   - OR any custom name like `portfolio`
3. Make it **Public**
4. Don't initialize with README (we already have one)

### Step 2: Push Your Code to GitHub

Open PowerShell in your project directory and run:

```powershell
# Initialize git repository
git init

# Add all files
git add .

# Commit changes
git commit -m "Initial commit: Personal portfolio website"

# Add remote repository (replace with your GitHub username)
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **Settings**
3. Scroll down to **Pages** section (left sidebar)
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**

Your site will be live at: `https://your-username.github.io/` or `https://your-username.github.io/repo-name/`

## 🌍 Setting Up .is-a.dev Domain

### Step 1: Fork the is-a-dev Repository

1. Go to [is-a-dev/register](https://github.com/is-a-dev/register)
2. Click **Fork** to create your own copy

### Step 2: Create Your Domain Configuration

1. In your forked repository, navigate to the `domains` folder
2. Create a new file: `your-subdomain.json` (e.g., `adiras.json`)
3. Add the following content:

```json
{
  "owner": {
    "username": "YOUR-GITHUB-USERNAME",
    "email": "your-email@example.com"
  },
  "record": {
    "CNAME": "YOUR-USERNAME.github.io"
  }
}
```

Example for you:
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

### Step 3: Submit Pull Request

1. Commit your changes
2. Create a **Pull Request** to the original is-a-dev repository
3. Wait for approval (usually takes 1-3 days)

### Step 4: Configure GitHub Pages for Custom Domain

Once your PR is approved:

1. Go to your GitHub repository **Settings** → **Pages**
2. Under **Custom domain**, enter: `your-subdomain.is-a.dev` (e.g., `adiras.is-a.dev`)
3. Click **Save**
4. Check **Enforce HTTPS** (after DNS propagation)

## 📝 Updating Your Website

To update your website:

```powershell
# Make your changes to the files

# Add changes
git add .

# Commit with a message
git commit -m "Update: Description of changes"

# Push to GitHub
git push origin main
```

GitHub Pages will automatically rebuild and deploy your site within a few minutes.

## 🎨 Customization Tips

### Update Personal Information
- Edit `index.html` to change content
- Replace images in `img/organization/` with your company logos
- Update `resume/Adiras_Resume.pdf` with your latest resume

### Change Colors
- Edit `css/main.css` to customize colors and styles
- Look for color codes (e.g., `#ffdc00`) and replace them

### Add New Sections
- Follow the existing HTML structure in `index.html`
- Use the `.section` class for consistent styling

## 📧 Contact

Feel free to reach out to me:
- **Email**: mr.adiras@gmail.com
- **LinkedIn**: [linkedin.com/in/adirassahu](https://linkedin.com/in/adirassahu)
- **GitHub**: [github.com/OxAdiras](https://github.com/OxAdiras)

## 📄 License

This project is open source and available for personal use. Feel free to fork and customize it for your own portfolio!

---

**Note**: Before deploying, make sure to:
1. Update all personal information in `index.html`
2. Add your own resume PDF in the `resume/` folder
3. Replace company logos with relevant ones in `img/organization/`
4. Test the website locally by opening `index.html` in a browser

Happy coding! 🚀
