# GitHub Deployment Guide

Follow these steps to deploy your Resume Optimizer app to GitHub Pages.

## Prerequisites

- A GitHub account (create one at https://github.com if you don't have one)
- Git installed on your computer (download from https://git-scm.com/)

## Step-by-Step Deployment

### 1. Create a New GitHub Repository

1. Go to https://github.com and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Name your repository (e.g., `resume-optimizer-app`)
5. Choose "Public" (required for free GitHub Pages)
6. Do NOT initialize with README, .gitignore, or license (we already have these)
7. Click "Create repository"

### 2. Initialize Local Git Repository

Open your terminal/command prompt and navigate to the project folder, then run:

```bash
# Navigate to the project directory
cd path/to/resume-optimizer-app

# Initialize git repository
git init

# Add all files
git add .

# Make your first commit
git commit -m "Initial commit: Resume Optimizer app"

# Add your GitHub repository as remote (replace YOUR_USERNAME and YOUR_REPO)
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" (top menu)
3. Click "Pages" in the left sidebar
4. Under "Source", select "Deploy from a branch"
5. Under "Branch", select "main" and "/ (root)"
6. Click "Save"

### 4. Access Your Live Site

After a few minutes, your site will be live at:
```
https://YOUR_USERNAME.github.io/YOUR_REPO/
```

For example: `https://johndoe.github.io/resume-optimizer-app/`

## Updating Your Site

Whenever you make changes:

```bash
git add .
git commit -m "Description of changes"
git push
```

GitHub Pages will automatically redeploy your site.

## Custom Domain (Optional)

If you want to use a custom domain:

1. In repository Settings > Pages
2. Enter your custom domain
3. Update your domain's DNS settings to point to GitHub Pages
4. See: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

## Troubleshooting

### Site not loading?
- Wait 5-10 minutes after enabling GitHub Pages
- Check Settings > Pages for any error messages
- Ensure your repository is public

### Changes not showing?
- GitHub Pages can take a few minutes to update
- Try clearing your browser cache
- Check the "Actions" tab in your repository to see deployment status

### 404 Error?
- Make sure the file is named `index.html` (lowercase)
- Verify the file is in the root directory
- Check that GitHub Pages is enabled in Settings

## Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Git Documentation](https://git-scm.com/doc)
- [GitHub Desktop](https://desktop.github.com/) - GUI alternative to command line

---

Need help? Create an issue in your repository or check the GitHub community forums.
