# NeuroFlow — Brain Reset Protocol
### Beta v0.1.0 · Progressive Web App

> **Science-backed 15-day dopamine reset app. Works on Android, iPhone, desktop, and laptop — installable without an app store.**

---

## ⚡ Deploy in 3 Minutes (GitHub Pages)

```bash
# 1. Create a new GitHub repo called "neuroflow"
# 2. Upload these 3 files:  index.html  /  sw.js  /  manifest.json
# 3. Go to: Settings → Pages → Source: main branch → / (root) → Save
# 4. Your app is live at: https://YOUR_USERNAME.github.io/neuroflow
```

---

## 📱 Install on Android (Google Play alternative — faster!)

### Method A: Direct PWA Install (No App Store needed — 30 seconds)
1. Open Chrome on Android
2. Navigate to your GitHub Pages URL
3. Tap the **"Install App"** banner that appears automatically
4. OR: Tap the 3-dot menu → **"Add to Home Screen"**
5. Done — it's on your home screen like a native app ✅

### Method B: Google Play Store (Official listing)
1. Deploy to GitHub Pages (step above) — you need an HTTPS URL
2. Go to **[pwabuilder.com](https://www.pwabuilder.com)**
3. Enter your GitHub Pages URL (e.g. `https://yourname.github.io/neuroflow`)
4. Click **Start** → **Package for Stores** → **Google Play**
5. Download the `.aab` (Android App Bundle)
6. Upload to [Google Play Console](https://play.google.com/console) → Create App → Internal Testing
7. Submit for review (takes 1–3 days for beta testing approval)

> **Cost:** Google Play Developer account = $25 one-time fee

---

## 💻 Install on Laptop / Desktop

### Chrome or Edge (Windows, Mac, Linux):
1. Open your GitHub Pages URL in Chrome or Edge
2. Look for the **install icon** (⊕) in the address bar (right side)
3. Click it → **Install**
4. App appears in your taskbar / dock / app launcher ✅

### Manual (any browser):
- Chrome: address bar → 3 dots → **"Install NeuroFlow"**
- Edge: address bar → 3 dots → **Apps → Install this site as an app**
- Safari (Mac): Share → **Add to Dock**

---

## 🍎 Install on iPhone / iPad

1. Open Safari on iPhone (must use Safari — not Chrome)
2. Navigate to your GitHub Pages URL
3. Tap the Share button (box with arrow)
4. Scroll down → **"Add to Home Screen"**
5. Tap **Add** → Done ✅

---

## 💾 Data Storage (Reliable & Persistent)

This app uses **IndexedDB** as primary storage with localStorage as fallback:

| Storage Type | Capacity | Persists | Works Offline |
|---|---|---|---|
| IndexedDB (primary) | 50MB–1GB | ✅ Yes | ✅ Yes |
| localStorage (fallback) | 5–10MB | ✅ Yes | ✅ Yes |

Your 15-day data is stored on your device. To back it up:
- Settings ⚙ → **Export Data** → Downloads a JSON file
- Import: coming in v0.2

**Important for longevity:** Don't clear browser/app data. If you reinstall the browser, export first.

---

## 🗂 File Structure

```
neuroflow/
├── index.html       ← Complete app (HTML + CSS + JS, self-contained)
├── manifest.json    ← PWA manifest (enables "Install App" button)
├── sw.js            ← Service Worker (offline caching)
└── README.md        ← This file
```

**Zero dependencies. No npm. No build step.**

---

## 🔧 Tech Stack

```
Frontend:    Pure HTML5 · CSS3 Custom Properties · Vanilla JS ES6+
Storage:     IndexedDB (primary) → localStorage (fallback)
Offline:     Service Worker (caches all files after first load)
Install:     Web App Manifest (PWA — installable on all platforms)
Fonts:       System fonts (works offline) + Google Fonts (enhancement)
Icons:       Inline SVG (no external files needed)
```


## ⚠️ Disclaimer

NeuroFlow is a wellness and education tool. Not medical advice. Consult a qualified healthcare professional before starting new health, supplement, or exercise protocols.

---

## 📄 License

MIT — free to use, fork, and build a business on. Attribution appreciated.

---

*Zero dependencies. Ships offline. Installs on every platform. Built on real neuroscience.* 🧠
