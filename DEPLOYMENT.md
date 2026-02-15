# Deployment Guide - FT Agritech Solutions Website

Complete guide to deploy your website to various hosting platforms.

## 🚀 Quick Deploy Options

### Option 1: Vercel (Recommended - Fastest)

**Why Vercel?**
- Free hosting for static sites
- Automatic HTTPS
- Global CDN
- Instant deployments
- Custom domain support

**Steps:**

1. **Install Vercel CLI** (if not already installed):
```bash
npm install -g vercel
```

2. **Navigate to your project folder**:
```bash
cd path/to/ft-agritech-website
```

3. **Deploy**:
```bash
vercel
```

4. **Follow the prompts**:
   - Login to Vercel (or create account)
   - Confirm project settings
   - Get your live URL instantly!

5. **For production deployment**:
```bash
vercel --prod
```

**Alternative: Deploy via Vercel Website**
1. Go to [vercel.com](https://vercel.com)
2. Click "New Project"
3. Import from Git or drag & drop your folder
4. Deploy!

---

### Option 2: Netlify

**Why Netlify?**
- Free tier with generous limits
- Drag-and-drop deployment
- Form handling built-in
- Easy custom domains

**Method A: Drag & Drop (Easiest)**

1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag your entire project folder
3. Done! Get your live URL

**Method B: Netlify CLI**

1. **Install Netlify CLI**:
```bash
npm install -g netlify-cli
```

2. **Login**:
```bash
netlify login
```

3. **Deploy**:
```bash
netlify deploy
```

4. **Deploy to production**:
```bash
netlify deploy --prod
```

**Enable Netlify Forms** (for contact form):
Add this to your form in `index.html`:
```html
<form name="contact" method="POST" data-netlify="true">
```

---

### Option 3: GitHub Pages

**Why GitHub Pages?**
- Free hosting
- Direct from GitHub repository
- Version control included

**Steps:**

1. **Create a GitHub repository**:
   - Go to [github.com](https://github.com)
   - Click "New Repository"
   - Name it (e.g., "ft-agritech-website")

2. **Push your code**:
```bash
git init
git add .
git commit -m "Initial commit - FT Agritech website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/ft-agritech-website.git
git push -u origin main
```

3. **Enable GitHub Pages**:
   - Go to repository Settings
   - Scroll to "Pages" section
   - Source: Select "main" branch
   - Click Save
   - Your site will be live at: `https://YOUR-USERNAME.github.io/ft-agritech-website/`

---

### Option 4: Firebase Hosting

**Why Firebase?**
- Google infrastructure
- Free SSL
- Fast global CDN

**Steps:**

1. **Install Firebase CLI**:
```bash
npm install -g firebase-tools
```

2. **Login**:
```bash
firebase login
```

3. **Initialize**:
```bash
firebase init hosting
```
   - Select "Use an existing project" or create new
   - Set public directory: `.` (current directory)
   - Configure as single-page app: No
   - Don't overwrite index.html

4. **Deploy**:
```bash
firebase deploy
```

---

### Option 5: Render

**Why Render?**
- Free static site hosting
- Auto-deploy from Git
- Custom domains

**Steps:**

1. Push code to GitHub (see GitHub Pages steps above)
2. Go to [render.com](https://render.com)
3. Click "New Static Site"
4. Connect your GitHub repository
5. Configure:
   - Build Command: (leave empty)
   - Publish Directory: `.`
6. Click "Create Static Site"

---

## 🌐 Custom Domain Setup

### For Vercel:
1. Go to your project dashboard
2. Click "Settings" → "Domains"
3. Add your custom domain
4. Update DNS records as instructed

### For Netlify:
1. Go to "Domain Settings"
2. Click "Add custom domain"
3. Follow DNS configuration steps

### For GitHub Pages:
1. Add a `CNAME` file with your domain:
```bash
echo "www.ftagritech.com" > CNAME
git add CNAME
git commit -m "Add custom domain"
git push
```
2. Configure DNS at your domain registrar

---

## 📧 Contact Form Integration

The current form has client-side validation only. To make it functional:

### Option A: Formspree (Easiest)

1. Go to [formspree.io](https://formspree.io)
2. Create free account
3. Create new form
4. Update form action in `index.html`:
```html
<form action="https://formspree.io/f/YOUR-FORM-ID" method="POST">
```

### Option B: EmailJS

1. Sign up at [emailjs.com](https://www.emailjs.com)
2. Create email service
3. Add EmailJS SDK to your HTML
4. Update JavaScript to use EmailJS

### Option C: Netlify Forms

If using Netlify, add to form:
```html
<form name="contact" method="POST" data-netlify="true">
```

### Option D: Custom Backend

Create a backend API using:
- Node.js + Express
- Python + Flask
- PHP
- Serverless functions (Vercel/Netlify)

---

## ✅ Pre-Deployment Checklist

- [ ] Test website locally (open index.html in browser)
- [ ] Check all links work
- [ ] Test contact form validation
- [ ] Verify responsive design on mobile
- [ ] Add real images to assets folder
- [ ] Update contact information (email, phone)
- [ ] Add real social media links
- [ ] Test on different browsers
- [ ] Optimize images (compress)
- [ ] Add favicon
- [ ] Update meta tags for SEO

---

## 🔧 Post-Deployment Tasks

1. **Add Analytics**:
   - Google Analytics
   - Vercel Analytics
   - Plausible Analytics

2. **SEO Optimization**:
   - Submit sitemap to Google Search Console
   - Add meta descriptions
   - Optimize images with alt text

3. **Performance**:
   - Test with Google PageSpeed Insights
   - Optimize images further if needed
   - Enable caching

4. **Security**:
   - Ensure HTTPS is enabled
   - Add security headers

---

## 🆘 Troubleshooting

**Issue: CSS not loading**
- Check file paths are correct
- Ensure files are in same directory
- Clear browser cache

**Issue: Form not submitting**
- Integrate with form service (see above)
- Check JavaScript console for errors

**Issue: Images not showing**
- Verify image paths
- Check file names match exactly (case-sensitive)
- Ensure images are in assets folder

**Issue: Mobile menu not working**
- Check JavaScript is loaded
- Verify script.js is linked correctly
- Check browser console for errors

---

## 📞 Support

For deployment issues:
- Vercel: [vercel.com/support](https://vercel.com/support)
- Netlify: [netlify.com/support](https://netlify.com/support)
- GitHub: [docs.github.com/pages](https://docs.github.com/pages)

---

**Built by AZAHELL TECH**

Good luck with your deployment! 🚀
