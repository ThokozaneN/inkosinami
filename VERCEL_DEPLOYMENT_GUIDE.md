# Vercel Deployment Guide for INkosinami NPO

This guide provides step-by-step instructions for deploying the INkosinami Drop-In Center website to Vercel.

## 1. Prerequisites
- A GitHub, GitLab, or Bitbucket account.
- A Vercel account (free tier is perfect).
- The project files ready (which they are!).

## 2. Push to GitHub
1. Create a new repository on your GitHub account (e.g., `inkosinami-website`).
2. Initialize git in your local project folder (if not already):
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Production ready"
   ```
3. Connect and push to your GitHub repo:
   ```bash
   git remote add origin https://github.com/your-username/inkosinami-website.git
   git branch -M main
   git push -u origin main
   ```

## 3. Deploy to Vercel
1. Log in to [Vercel.com](https://vercel.com).
2. Click **"Add New"** -> **"Project"**.
3. Select your GitHub repository from the list.
4. **Configure Project**:
   - **Framework Preset**: Vite (should be auto-detected).
   - **Build Command**: `npm run build`
   - **Output Directory**: `dist`
   - **Install Command**: `npm install`
5. Click **"Deploy"**.

## 4. Why Vercel?
- **Global CDN**: Your site will be lightning-fast across South Africa and the world.
- **Auto-Deploy**: Every change you push to GitHub will automatically update the live site.
- **SSL by Default**: The site will be secured with HTTPS automatically.
- **Analytics**: Vercel provides great insights into site performance.

## 5. Post-Deployment Checklist
- [ ] Connect a custom domain (e.g., `inkosinami.org`) in the Vercel project settings.
- [ ] Verify that all GSAP animations run smoothly on the production URL.
- [ ] Test the "Copy Bank Details" functionality on a mobile device.

---
**Prepared with ❤️ for INkosinami Drop-In Center.**
