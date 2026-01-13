# PRINT3D-LAB Service Maintenance PWA

## 📱 What's Included

```
print3d-lab-pwa/
├── index.html          # Main application
├── manifest.json       # PWA configuration
├── sw.js              # Service Worker (offline support)
└── icons/             # App icons for all devices
    ├── icon-72x72.png
    ├── icon-96x96.png
    ├── icon-128x128.png
    ├── icon-144x144.png
    ├── icon-152x152.png
    ├── icon-192x192.png
    ├── icon-384x384.png
    └── icon-512x512.png
```

## 🚀 Deployment Options

### Option 1: GitHub Pages (FREE - Recommended)

1. Create a GitHub account (if you don't have one)
2. Create a new repository named `print3d-lab-service`
3. Upload all files from the ZIP
4. Go to Settings → Pages → Source: "main" branch
5. Your app will be live at: `https://yourusername.github.io/print3d-lab-service`

### Option 2: Netlify (FREE)

1. Go to netlify.com and sign up
2. Drag and drop the extracted folder to deploy
3. Your app will be live instantly with a free URL

### Option 3: Local Web Server

For testing locally, you can use:

```bash
# Python 3
cd print3d-lab-pwa
python -m http.server 8000
# Then open http://localhost:8000

# Or with Node.js
npx serve
```

**Note:** PWA features (install prompt, offline) require HTTPS or localhost.

## 📲 Installing on Your Phone

### Android (Chrome)
1. Open the app URL in Chrome
2. You'll see an "Install" banner at the bottom
3. Tap "Install" or go to Menu (⋮) → "Install app" or "Add to Home screen"
4. The app icon will appear on your home screen

### iPhone (Safari)
1. Open the app URL in Safari
2. Tap the Share button (square with arrow)
3. Scroll down and tap "Add to Home Screen"
4. Tap "Add" in the top right

## 🔄 Converting to APK (Optional)

If you want a real Android APK:

1. Deploy your PWA to a public URL (GitHub Pages, Netlify, etc.)
2. Go to https://www.pwabuilder.com/
3. Enter your PWA URL
4. Click "Package for Stores"
5. Download the Android APK
6. Install on your phone (enable "Unknown Sources" in settings)

## ✨ Features

- ✅ Works offline (after first load)
- ✅ Installs like a native app
- ✅ Full-screen mode (no browser UI)
- ✅ Auto-save drafts to browser storage
- ✅ PDF generation with photos
- ✅ Email integration with pre-filled template
- ✅ Camera and photo upload support
- ✅ Multiple machine support
- ✅ Color-coded status indicators

## 🔧 Customization

### Change Technician Info
Edit `index.html` and find the `technicians` object:

```javascript
const technicians = {
    nereo: {
        name: 'Nereo Gil',
        phone: '0473071215',
        email: 'nereo@print3dlab.com.au'
    }
    // Add more technicians here
};
```

### Change Colors
Edit the CSS variables at the top of `index.html`:

```css
:root {
    --primary: #1a1a2e;
    --accent: #e94560;
    /* etc. */
}
```

## 📞 Support

For issues or feature requests, contact:
- Email: nereo@print3dlab.com.au
- Phone: 0473071215

---

**PRINT3D-LAB** - Precision in Every Layer
