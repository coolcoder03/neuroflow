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

---

## 🚀 Roadmap to Production

### v0.2 (Week 2–3)
- [ ] Push notifications for daily habit reminders (Web Push API)
- [ ] NSDR audio tracks (Howler.js, hosted audio files)
- [ ] Import/restore from JSON backup
- [ ] Share completion badges (Web Share API)
- [ ] Apple App Store via PWABuilder

### v0.3 (Month 1)
- [ ] Supabase backend (cloud sync across devices)
- [ ] User accounts (email or Google)
- [ ] Community wall ("Day 10 complete!")
- [ ] Coach/accountability partner feature

### v1.0 (Month 2–3)
- [ ] AI scheduler (Claude/OpenAI API) — personalised daily order
- [ ] Apple Health / Google Fit integration
- [ ] Stripe payment for Pro tier ($9/month)
- [ ] Enterprise team dashboard

---

## 💼 Business Model

```
Free:        Full 15-day plan · 4 brain games · habit tracker · timers
Pro ($9/mo): AI scheduling · NSDR audio library · cloud sync · analytics
Teams ($12/user/mo): HR dashboard · Slack bot · burnout prevention reports
```

**To add Stripe payments:**
```html
<script src="https://js.stripe.com/v3/"></script>
```
Add a paywall check before rendering Day 6+ content in the `renderPlanDay()` function.

**To add cloud sync (Supabase — free tier):**
```js
// Replace the DB.set/DB.get calls with:
await supabase.from('progress').upsert({ user_id, key, value });
```
The DB storage object is already abstracted — just swap the implementation.

---

## 📡 Science Sources

1. **Dr. Sanil Rege** (PsychScene) — *Procrastination Is a Dopamine Timing Problem* · youtu.be/lacFcgcHx6I
2. **Dr. Andrew Huberman** (Stanford) — *Leverage Dopamine to Overcome Procrastination* · Huberman Lab
3. **Šrámek et al.** — Cold water immersion +250% dopamine (European J. Applied Physiology, 2000)
4. **Erickson et al.** — Exercise increases hippocampal volume (PNAS, 2011)
5. **Stickgold & Walker** — Sleep/NSDR and neuroplasticity (Neuron, 2013)
6. **Shurtleff et al.** — Tyrosine improves working memory (Pharmacology Biochemistry, 1994)
7. **Schultz** — Dopamine reward prediction error (Current Opinion in Neurobiology, 2020)
8. **Jaeggi et al.** — N-Back training and fluid intelligence (PNAS, 2008)
9. **Dr. Anna Lembke** — Dopamine Nation (Stanford, 2021)
10. **Aron et al.** — PFC inhibitory control (Nature Reviews Neuroscience, 2007)

---

## ⚠️ Disclaimer

NeuroFlow is a wellness and education tool. Not medical advice. Consult a qualified healthcare professional before starting new health, supplement, or exercise protocols.

---

## 📄 License

MIT — free to use, fork, and build a business on. Attribution appreciated.

---

*Zero dependencies. Ships offline. Installs on every platform. Built on real neuroscience.* 🧠
