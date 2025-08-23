# 🚀 Quick Deployment Guide

## Deploy to GitHub Pages in 5 Minutes

### Step 1: Create GitHub Repository
1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Name it: `developer-portfolio-template` (or your preferred name)
5. Make it **Public** (required for free GitHub Pages)
6. Don't initialize with README (we already have one)
7. Click "Create repository"

### Step 2: Upload Your Files
**Option A: Using Git (Recommended)**
```bash
# Open terminal/command prompt in your project folder
git init
git add .
git commit -m "Initial portfolio commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/developer-portfolio-template.git
git push -u origin main
```

**Option B: Using GitHub Web Interface**
1. In your new repository, click "uploading an existing file"
2. Drag and drop all your project files
3. Click "Commit changes"

### Step 3: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click **Settings** tab
3. Scroll down to **Pages** section (in the left sidebar)
4. Under **Source**, select **Deploy from a branch**
5. Choose **main** branch and **/ (root)** folder
6. Click **Save**

### Step 4: Wait for Deployment
- GitHub will show a blue banner: "Your site is being built"
- Wait 2-5 minutes for deployment
- You'll see a green checkmark when ready

### Step 5: Your Site is Live! 🎉
Your portfolio will be available at:
`https://sohail7739.github.io/CodeWithSohail`

## 🔧 Custom Domain (Optional)
If you want a custom domain like `yourname.com`:
1. Buy a domain from any registrar
2. In GitHub Pages settings, add your custom domain
3. Update your domain's DNS settings
4. Wait for DNS propagation (up to 24 hours)

## 📧 Fix Contact Form
Since GitHub Pages doesn't support PHP, replace the contact form with:

**Option A: Formspree (Free)**
1. Go to [Formspree.io](https://formspree.io)
2. Create a free account
3. Create a new form
4. Replace the form action in `index.html` with your Formspree endpoint

**Option B: Netlify Forms**
1. Deploy to Netlify instead
2. Add `netlify` attribute to your form
3. Forms will work automatically

## 🎨 Customize Your Portfolio
Before deploying, update:
- Your name and title in `index.html`
- About section content
- Portfolio projects
- Contact information
- Profile pictures in `img/` folder

## 🔄 Update Your Site
After making changes:
```bash
git add .
git commit -m "Update portfolio"
git push
```
GitHub Pages will automatically rebuild and deploy your changes!

## 🆘 Troubleshooting
- **Site not loading?** Check if repository is public
- **Images not showing?** Make sure all image paths are correct
- **Contact form not working?** Set up Formspree or Netlify Forms
- **Styling issues?** Check browser console for errors

## 📞 Need Help?
- Check GitHub Pages documentation
- Look at the Actions tab for deployment status
- Ensure all files are in the root directory
