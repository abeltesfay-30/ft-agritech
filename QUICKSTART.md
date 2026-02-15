# Quick Start Guide - FT Agritech Solutions Website

Get your website up and running in 5 minutes!

## 📦 What You Have

Your complete website package includes:
- ✅ `index.html` - Main website file
- ✅ `style.css` - All styling and responsive design
- ✅ `script.js` - Interactive features and animations
- ✅ `assets/` - Folder for images and icons
- ✅ `README.md` - Full documentation
- ✅ `DEPLOYMENT.md` - Deployment instructions
- ✅ `vercel.json` - Vercel configuration

## 🚀 3 Ways to View Your Website

### Method 1: Open Directly (Instant)
1. Navigate to your project folder
2. Double-click `index.html`
3. Website opens in your default browser
4. ✅ Done!

### Method 2: Use Live Server (Recommended for Development)
1. Install [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in VS Code
2. Right-click `index.html`
3. Select "Open with Live Server"
4. Auto-refreshes when you make changes!

### Method 3: Python Simple Server
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```
Then open: `http://localhost:8000`

## 🎨 Customize Your Website

### 1. Update Contact Information

**File:** `index.html`

Find and replace:
```html
<!-- Line ~580 -->
<p>ft.agritech@gmail.com</p>
<p>+251 XXX XXX XXX</p>
```

With your actual contact details.

### 2. Add Your Logo

1. Save your logo as `logo.png` in `assets/images/`
2. Update `index.html`:
```html
<!-- Replace line ~20 -->
<div class="logo">
    <img src="assets/images/logo.png" alt="FT Agritech" style="height: 40px;">
</div>
```

### 3. Add Social Media Links

**File:** `index.html` (around line ~600)

```html
<div class="social-links">
    <a href="https://facebook.com/yourpage" class="social-icon">📘</a>
    <a href="https://twitter.com/yourhandle" class="social-icon">🐦</a>
    <a href="https://linkedin.com/company/yourcompany" class="social-icon">💼</a>
    <a href="https://instagram.com/yourhandle" class="social-icon">📷</a>
</div>
```

### 4. Change Colors

**File:** `style.css` (lines 7-15)

```css
:root {
    --primary-green: #2ecc71;    /* Change this */
    --tech-blue: #3498db;        /* Change this */
    /* Your custom colors */
}
```

### 5. Add Images

1. Place images in `assets/images/`
2. Reference in HTML:
```html
<img src="assets/images/your-image.jpg" alt="Description">
```

## 🌐 Deploy to Internet (Choose One)

### Fastest: Vercel (2 minutes)
```bash
npm install -g vercel
vercel
```
Follow prompts → Get live URL!

### Easiest: Netlify Drop
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag your folder
3. Done!

### Free: GitHub Pages
```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin YOUR-REPO-URL
git push -u origin main
```
Enable Pages in repo settings.

**See DEPLOYMENT.md for detailed instructions.**

## 📧 Make Contact Form Work

The form currently has validation only. To receive emails:

### Option 1: Formspree (Easiest - 2 minutes)
1. Go to [formspree.io](https://formspree.io)
2. Sign up free
3. Create form → Get form ID
4. Update `index.html` line ~605:
```html
<form action="https://formspree.io/f/YOUR-FORM-ID" method="POST" id="contactForm">
```

### Option 2: Netlify Forms (If using Netlify)
Add to form tag:
```html
<form data-netlify="true" name="contact" method="POST">
```

## ✅ Pre-Launch Checklist

Before going live:
- [ ] Replace placeholder contact info
- [ ] Add real email and phone number
- [ ] Update social media links
- [ ] Add your logo
- [ ] Add product/team images
- [ ] Test contact form
- [ ] Test on mobile device
- [ ] Check all sections load properly
- [ ] Add favicon (optional)

## 🎯 Key Features Already Built-In

✅ Fully responsive (mobile, tablet, desktop)  
✅ Smooth scroll navigation  
✅ Animated statistics counters  
✅ Contact form with validation  
✅ Success modal popup  
✅ Sticky navigation bar  
✅ Scroll animations  
✅ Mobile hamburger menu  
✅ Professional design  
✅ Fast loading  

## 📱 Test Responsiveness

1. Open website in browser
2. Press `F12` (Developer Tools)
3. Click device icon (toggle device toolbar)
4. Test different screen sizes:
   - iPhone SE (375px)
   - iPad (768px)
   - Desktop (1200px+)

## 🔧 Common Customizations

### Change Hero Background
**File:** `style.css` (line ~95)
```css
.hero {
    background: url('assets/images/hero-bg.jpg');
}
```

### Update Company Name
Find and replace "FT Agritech Solutions" throughout `index.html`

### Modify Statistics
**File:** `index.html` (lines ~150-170)
```html
<div class="stat-number" data-target="240">0</div>
```
Change `data-target` value.

### Add New Section
Copy any existing section structure and modify content.

## 📚 File Structure

```
ft-agritech-website/
├── index.html          ← Main website
├── style.css           ← All styles
├── script.js           ← Functionality
├── assets/
│   ├── images/         ← Add images here
│   └── icons/          ← Add icons here
├── README.md           ← Full documentation
├── DEPLOYMENT.md       ← Deploy guide
├── QUICKSTART.md       ← This file
└── vercel.json         ← Vercel config
```

## 🆘 Need Help?

**Website not loading?**
- Check all files are in same folder
- Try different browser
- Clear browser cache

**Styles not working?**
- Verify `style.css` is in same folder as `index.html`
- Check file names match exactly

**JavaScript not working?**
- Check `script.js` is in same folder
- Open browser console (F12) for errors

**Form not submitting?**
- Integrate with Formspree or Netlify Forms
- See "Make Contact Form Work" section above

## 🎉 You're Ready!

Your professional AgriTech startup website is ready to launch!

**Next Steps:**
1. Customize content (5 minutes)
2. Add images (10 minutes)
3. Deploy to internet (2 minutes)
4. Share with the world! 🚀

---

**Built by AZAHELL TECH**

Questions? Check README.md and DEPLOYMENT.md for more details.
