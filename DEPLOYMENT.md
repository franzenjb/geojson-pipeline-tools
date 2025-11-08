# Deployment Guide

## 🚀 Deploying to GitHub Pages

This repository is set up for automatic deployment to GitHub Pages. Follow these steps:

### First Time Setup

1. **Create the GitHub repository** (if not already created):
   ```bash
   # On GitHub.com, create a new repository named "geojson-pipeline-tools"
   # Make it public (required for free GitHub Pages)
   ```

2. **Commit and push your code**:
   ```bash
   cd /Users/jefffranzen/geojson-pipeline-tools
   
   # Initial commit
   git add -A
   git commit -m "Initial commit: GeoJSON Pipeline Tools"
   
   # Add remote (replace YOUR_USERNAME if different)
   git remote add origin https://github.com/franzenjb/geojson-pipeline-tools.git
   
   # Push to GitHub
   git branch -M main
   git push -u origin main
   ```

3. **Enable GitHub Pages**:
   - Go to your repository on GitHub.com
   - Click **Settings** → **Pages**
   - Under **Source**, select **GitHub Actions**
   - The workflow will automatically deploy when you push to `main`

### Automatic Deployment

Once set up, every time you push to the `main` branch:
- GitHub Actions will automatically build and deploy
- Your site will be live at: `https://franzenjb.github.io/geojson-pipeline-tools/`
- Deployment typically takes 1-2 minutes

### Verify Deployment

After pushing, check:
1. **GitHub Actions**: Go to the **Actions** tab to see deployment status
2. **Live Site**: Visit `https://franzenjb.github.io/geojson-pipeline-tools/`
3. **Portfolio Link**: The portfolio showcase will automatically use the web version

### Troubleshooting

- **404 Error**: Wait a few minutes for GitHub Pages to propagate
- **Actions Failing**: Check the Actions tab for error messages
- **Site Not Updating**: Clear browser cache or wait for CDN propagation

