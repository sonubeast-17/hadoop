# Vercel Deployment Guide

## Method 1: Vercel CLI (Recommended)

### Prerequisites
- Node.js installed on your computer
- Vercel account (free)

### Steps:
1. **Install Vercel CLI**:
   ```bash
   npm install -g vercel
   ```

2. **Login to Vercel**:
   ```bash
   vercel login
   ```

3. **Deploy from your project folder**:
   ```bash
   cd c:/Users/konda/OneDrive/Documents/231FA18454/BDA_FLAPPY
   vercel
   ```

4. **Follow the prompts**:
   - Set up and deploy? → **Yes**
   - Which scope? → Choose your Vercel account
   - Link to existing project? → **No** (first time)
   - Project name? → **flappy-game** (or your choice)
   - In which directory is your code located? → **./** (current directory)
   - Want to override settings? → **No**

5. **Your site is live!** Vercel will give you a URL like `https://flappy-game.vercel.app`

## Method 2: Vercel Web Dashboard

### Steps:
1. **Go to [vercel.com](https://vercel.com)** and sign up/login
2. **Click "Add New..." → "Project"**
3. **Import Git Repository**:
   - Choose "Git Repository" tab
   - Import from GitHub/GitLab/Bitbucket
   - Or use "Git Integration" to connect your local repo
4. **Configure Project**:
   - Framework Preset: **Other**
   - Root Directory: Leave empty
   - Build Command: Leave empty (static site)
   - Output Directory: Leave empty
   - Install Command: Leave empty
5. **Click "Deploy"**

## Method 3: Drag & Drop (Easiest)

### Steps:
1. **Go to [vercel.com](https://vercel.com)**
2. **Drag your entire BDA_FLAPPY folder onto the dashboard**
3. **Wait for deployment** (usually 1-2 minutes)
4. **Get your URL**

## After Deployment

### Updating Your Game:
- **Method 1**: Run `vercel --prod` in your project folder
- **Method 2**: Push changes to Git, Vercel auto-deploys
- **Method 3**: Re-drag the updated folder

### Custom Domain (Optional):
1. Go to your project dashboard on Vercel
2. Click "Settings" → "Domains"
3. Add your custom domain

## Troubleshooting

### Common Issues:
- **Audio not working**: Browser requires user interaction first (click/tap)
- **Images not loading**: Check file names and paths
- **Build errors**: This is a static site - no build needed

### Deployment Status:
- Your game is configured as a static site
- No build process required
- All assets (images, audio) are included
- Ready for immediate deployment

## Files Included:
- `index.html` - Main game file
- `bird.png` - Bird and pipe image
- `hadoop.ogg` - Jump sound
- `internship.ogg` - Game over sound
- `vercel.json` - Vercel configuration
- `package.json` - Project metadata

Your game is ready for deployment! 🎮
