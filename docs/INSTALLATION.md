# Installation Guide - AgroConnect

This guide will walk you through the installation and setup process for the AgroConnect project.

---

## 📋 System Requirements

### Minimum Requirements
- **OS:** Windows, macOS, or Linux
- **Browser:** Any modern browser (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- **RAM:** 512 MB
- **Disk Space:** 100 MB

### Recommended Setup
- **OS:** Ubuntu 20.04+ / Windows 10+ / macOS 10.15+
- **IDE:** Visual Studio Code (Free)
- **Node.js:** 14.0+ (for future backend integration)
- **Git:** 2.25+

---

## 🚀 Installation Steps

### Option 1: Clone from GitHub (Recommended)

#### Step 1: Install Git
```bash
# Windows (using Chocolatey)
choco install git

# macOS (using Homebrew)
brew install git

# Linux (Ubuntu/Debian)
sudo apt-get install git
```

#### Step 2: Clone the Repository
```bash
git clone https://github.com/yourusername/AgroConnect.git
cd AgroConnect
```

#### Step 3: Open in VS Code
```bash
code .
```

#### Step 4: Start Development Server
```bash
# Install a simple HTTP server (if not already installed)
npm install -g http-server

# Run the server
http-server
```

Then open your browser to `http://localhost:8080`

---

### Option 2: Direct Download

1. Download the ZIP file from GitHub
2. Extract the ZIP file to your desired location
3. Open the folder in your code editor
4. Right-click on `index.html` → Open with → Browser

---

## 📂 Folder Setup

After cloning/extracting, your folder structure should look like:

```
AgroConnect/
├── 01-HTML/          ✓
├── 02-CSS/           ✓
├── 03-script/        ✓
├── 04-assets/        ✓
├── docs/             ✓ (Documentation)
├── AgroConnect/      ✓ (Assets folder)
├── index.html        ✓
├── style.css         ✓
├── README.md         ✓
└── .git/             ✓
```

---

## 🎯 Quick Start Options

### Option A: Run Directly in Browser (No Server Needed)
```bash
# Simply open the file
index.html
```
→ Double-click on index.html to open in your default browser

### Option B: Using Python (Built-in on Most Systems)
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```
→ Open `http://localhost:8000` in your browser

### Option C: Using Node.js
```bash
# Install http-server
npm install -g http-server

# Run server
http-server

# Or using live-server for live reloading
npm install -g live-server
live-server
```

### Option D: Using Visual Studio Code Live Server
1. Install "Live Server" extension by Ritwick Dey
2. Right-click on `index.html`
3. Select "Open with Live Server"

---

## 🔧 Configuration

### Basic Configuration (index.html)
Update the following if needed:
```html
<!-- Language setting -->
<button class="lang">EN</button>  <!-- Change to your language code -->

<!-- Logo image path -->
<img src="./04-assets/final-text-logo-1.png" alt="">

<!-- Links to pages -->
<a href="./01-HTML/about.html">About</a>
```

### CSS Customization (style.css)
```css
/* Update color scheme */
:root {
  --primary-color: #2ecc71;      /* Green for organic theme */
  --secondary-color: #27ae60;
  --text-color: #333;
  --background-color: #f5f5f5;
}
```

### JavaScript Configuration (03-script/script.js)
Update any API endpoints or configuration variables in this file when backend integration is added.

---

## 📱 Testing the Installation

### Desktop Testing
1. Open `index.html` in your browser
2. Navigate through all pages using the menu
3. Check responsive design: Right-click → Inspect → Toggle device toolbar

### Mobile/Tablet Testing
1. Use browser DevTools responsive mode (F12 → Click responsive button)
2. Test on physical devices if available
3. Common screen sizes to test:
   - **Mobile:** 375px × 667px (iPhone)
   - **Tablet:** 768px × 1024px (iPad)
   - **Desktop:** 1920px × 1080px (Full HD)

### Links Verification
Visit each page to verify:
- ✓ Navigation menu works
- ✓ All images load correctly
- ✓ Links navigate to correct pages
- ✓ Form elements are visible
- ✓ Responsive design on mobile

---

## 🐛 Troubleshooting

### Issue: Pages not loading
**Solution:**
- Check file paths in HTML files
- Ensure all files are in the correct folders
- Try using absolute URLs instead of relative paths

### Issue: CSS not applying
**Solution:**
- Clear browser cache (Ctrl+Shift+Delete)
- Check CSS file paths in HTML `<link>` tags
- Open DevTools (F12) → Sources tab to verify files load

### Issue: Images not displaying
**Solution:**
- Verify image file paths are correct
- Check if image files exist in `04-assets/` folder
- Use absolute paths: `/04-assets/image-name.jpg`

### Issue: Server not starting
**Solution:**
```bash
# Kill any process using the port
# Windows
netstat -ano | findstr :8000
taskkill /PID <PID> /F

# macOS/Linux
lsof -ti:8000 | xargs kill -9
```

### Issue: Port already in use
**Solution:**
```bash
# Use a different port
http-server -p 3000
python -m http.server 3001
```

---

## 🔐 Security Considerations

Currently, AgroConnect is a static website. When adding backend:

1. **Use HTTPS** for all connections
2. **Validate input** on both frontend and backend
3. **Protect sensitive data** (passwords, payment info)
4. **Use environment variables** for API keys
5. **Enable CORS** properly
6. **Implement authentication** securely
7. **Regular security audits** and updates

---

## 📦 Dependencies (Current)

### Frontend-Only (No Installation Needed)
- Font Awesome 7.0.1 (CDN)
- Google Fonts (CDN)
- Vanilla HTML/CSS/JavaScript

### When Adding Backend (Future)
- Node.js or Python (web framework)
- Database (MongoDB, PostgreSQL, MySQL)
- API library (Express.js, Flask, etc.)
- Package manager (npm, pip)

---

## 🚀 Deploying to GitHub Pages

1. Push your repository to GitHub:
```bash
git add .
git commit -m "Initial AgroConnect setup"
git push origin main
```

2. Go to repository settings → Pages
3. Select main branch as source
4. Your site will be live at: `https://yourusername.github.io/AgroConnect/`

---

## 📚 Additional Resources

- [VS Code Documentation](https://code.visualstudio.com/docs)
- [HTML Reference](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [JavaScript Guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide)
- [Git Guide](https://git-scm.com/doc)

---

## ✅ Installation Checklist

- [ ] Git installed and configured
- [ ] Repository cloned/downloaded
- [ ] Folder structure verified
- [ ] Web server running
- [ ] index.html opens in browser
- [ ] All pages load correctly
- [ ] Images display properly
- [ ] Responsive design works on mobile
- [ ] Navigation menu functions
- [ ] No console errors (F12)

---

## 🆘 Need Help?

1. Check GitHub Issues: `https://github.com/yourusername/AgroConnect/issues`
2. Review troubleshooting section above
3. Check SEO and keywords documentation
4. Contact project maintainers

---

**Last Updated:** March 2026  
**Status:** Installation Guide v1.0
