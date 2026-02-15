# 🧪 Test Your Website Locally

Quick guide to view and test your website before deploying.

## Method 1: Double-Click (Easiest)

1. Open your project folder
2. Find `index.html`
3. Double-click it
4. Website opens in your default browser
5. ✅ Done!

**Note:** Some features like form submission may not work fully without a server.

---

## Method 2: VS Code Live Server (Recommended)

### Install Live Server Extension

1. Open VS Code
2. Click Extensions icon (or press `Ctrl+Shift+X`)
3. Search for "Live Server"
4. Install "Live Server" by Ritwick Dey
5. Reload VS Code

### Run Live Server

1. Open your project folder in VS Code
2. Right-click on `index.html`
3. Select "Open with Live Server"
4. Website opens at `http://localhost:5500`
5. ✅ Auto-refreshes when you save changes!

**Benefits:**
- Auto-reload on save
- Works like a real server
- Better for testing

---

## Method 3: Python Simple Server

### If you have Python installed:

**Python 3:**
```bash
python -m http.server 8000
```

**Python 2:**
```bash
python -m SimpleHTTPServer 8000
```

Then open: `http://localhost:8000`

---

## Method 4: Node.js http-server

### If you have Node.js installed:

1. Install http-server globally:
```bash
npm install -g http-server
```

2. Run in your project folder:
```bash
http-server
```

3. Open: `http://localhost:8080`

---

## Method 5: PHP Built-in Server

### If you have PHP installed:

```bash
php -S localhost:8000
```

Then open: `http://localhost:8000`

---

## 🧪 What to Test

### Navigation
- [ ] Click all menu links
- [ ] Test smooth scrolling
- [ ] Check active link highlighting
- [ ] Test mobile hamburger menu

### Sections
- [ ] Hero section loads properly
- [ ] All sections are visible
- [ ] Images load (if added)
- [ ] Text is readable
- [ ] Colors look good

### Animations
- [ ] Scroll down slowly
- [ ] Watch counters animate
- [ ] Check progress bar fills
- [ ] Verify card animations
- [ ] Test hover effects

### Contact Form
- [ ] Try submitting empty form (should show validation)
- [ ] Enter invalid email (should show error)
- [ ] Fill all fields correctly
- [ ] Check success modal appears
- [ ] Verify form resets

### Responsive Design
- [ ] Resize browser window
- [ ] Test at different widths
- [ ] Check mobile menu appears < 768px
- [ ] Verify layout adjusts properly

### Browser Testing
- [ ] Chrome
- [ ] Firefox
- [ ] Safari (if on Mac)
- [ ] Edge

---

## 🔍 Check Browser Console

1. Press `F12` (or `Ctrl+Shift+I`)
2. Click "Console" tab
3. Look for any errors (red text)
4. Should see green FT Agritech message

**Expected Console Output:**
```
🌱 FT Agritech Solutions
Protecting Harvests with Smart IoT Crop Defense
Built by AZAHELL TECH
```

---

## 📱 Test Mobile View

### In Browser (Chrome/Firefox)

1. Press `F12` to open DevTools
2. Click device icon (toggle device toolbar)
3. Select device:
   - iPhone SE (375px)
   - iPhone 12 Pro (390px)
   - iPad (768px)
   - iPad Pro (1024px)
4. Test in portrait and landscape

### On Real Device

1. Find your computer's local IP:
   - Windows: `ipconfig`
   - Mac/Linux: `ifconfig`
2. Start local server (Method 2-5 above)
3. On phone, open browser
4. Go to: `http://YOUR-IP:PORT`
   - Example: `http://192.168.1.100:8000`

---

## ✅ Testing Checklist

### Visual
- [ ] All sections load
- [ ] Colors look correct
- [ ] Fonts are readable
- [ ] Spacing looks good
- [ ] No overlapping elements

### Functional
- [ ] Navigation works
- [ ] Smooth scroll works
- [ ] Animations play
- [ ] Form validation works
- [ ] Modal appears

### Responsive
- [ ] Mobile menu works
- [ ] Layout adjusts properly
- [ ] Text is readable on mobile
- [ ] Buttons are clickable
- [ ] No horizontal scroll

### Performance
- [ ] Page loads quickly
- [ ] Animations are smooth
- [ ] No lag when scrolling
- [ ] Images load fast

---

## 🐛 Common Issues & Fixes

### Issue: CSS not loading
**Fix:** 
- Check `style.css` is in same folder as `index.html`
- Clear browser cache (`Ctrl+Shift+R`)
- Check file name spelling

### Issue: JavaScript not working
**Fix:**
- Check `script.js` is in same folder
- Open console (F12) for errors
- Verify file name is correct

### Issue: Images not showing
**Fix:**
- Check image paths in HTML
- Verify images are in `assets/images/`
- Check file names match exactly (case-sensitive)

### Issue: Form not submitting
**Fix:**
- This is normal for local testing
- Form needs backend integration
- See DEPLOYMENT.md for form services

### Issue: Animations not playing
**Fix:**
- Scroll down slowly
- Refresh page
- Check if JavaScript is enabled
- Try different browser

---

## 🎯 Quick Test Script

Run through this in 2 minutes:

1. ✅ Open website
2. ✅ Scroll through all sections
3. ✅ Click each menu item
4. ✅ Test mobile menu (resize window)
5. ✅ Fill out contact form
6. ✅ Check console for errors
7. ✅ Test on mobile device

---

## 📊 Performance Testing

### Google PageSpeed Insights

1. Deploy to internet first (see DEPLOYMENT.md)
2. Go to: https://pagespeed.web.dev/
3. Enter your URL
4. Check scores (aim for 90+)

### Lighthouse (Built into Chrome)

1. Press `F12`
2. Click "Lighthouse" tab
3. Click "Generate report"
4. Review scores

---

## 🎨 Visual Testing

### Check These Elements

**Hero Section:**
- [ ] Title is large and readable
- [ ] Buttons are visible
- [ ] Background looks good

**About Section:**
- [ ] Stats animate when scrolled into view
- [ ] Text is well-formatted
- [ ] Cards look professional

**Problem Section:**
- [ ] Icons display correctly
- [ ] Cards have hover effect
- [ ] Layout is balanced

**Solution Section:**
- [ ] Feature cards are aligned
- [ ] Icons are visible
- [ ] Hover effects work

**Contact Section:**
- [ ] Form is centered
- [ ] Fields are properly sized
- [ ] Button is prominent

**Footer:**
- [ ] "Built by AZAHELL TECH" is visible
- [ ] Links work
- [ ] Layout is clean

---

## 💡 Pro Tips

1. **Test in Incognito Mode** - Ensures no cached files
2. **Use Multiple Browsers** - Catch compatibility issues
3. **Test on Real Devices** - Better than emulators
4. **Check at Different Times** - Test performance
5. **Get Feedback** - Ask others to test

---

## 🚀 Ready for Deployment?

Once local testing is complete:

1. ✅ All sections work
2. ✅ No console errors
3. ✅ Responsive on all devices
4. ✅ Animations are smooth
5. ✅ Form validation works

**Next Step:** See `DEPLOYMENT.md` to go live!

---

## 📞 Need Help?

Check these files:
- `README.md` - Full documentation
- `QUICKSTART.md` - Quick start guide
- `DEPLOYMENT.md` - Deploy instructions
- `LAUNCH_CHECKLIST.md` - Pre-launch checklist

---

**Built by AZAHELL TECH**

Happy testing! 🧪
