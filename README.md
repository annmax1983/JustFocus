# JustFocus

English | [中文](languages/README_zh.md) | [日本語](languages/README_ja.md) | [Deutsch](languages/README_de.md) | [Español](languages/README_es.md) | [Français](languages/README_fr.md)

A lightweight browser extension that blocks distracting websites to help you stay focused. Minimal, fast, and privacy-first.

> Chromium-based · Manifest V3 · Minimal Permissions · Local Only · No Tracking

---

## Why JustFocus?

Most site blockers are bloated with ads, forced sign-ups, and invasive tracking. JustFocus is different — it does one thing and does it well: **block the sites that distract you**.

| Advantage | Detail |
|-----------|--------|
| 🎯 **Single Purpose** | Block distracting sites. That's it. No bloat. |
| 🔒 **No Tracking** | No analytics, no accounts, no data collection whatsoever |
| ⚡ **Lightweight** | Under 50KB total. No frameworks, no dependencies. |
| 🕐 **Temp Bypass** | Need 5 minutes? Bypass a site temporarily without removing it |
| 🔄 **Global Toggle** | Pause all blocking with one switch — lunch break, weekends |
| 🌍 **6 Languages** | English, Chinese, Japanese, German, Spanish, French |

---

## Features

| Feature | Description |
|---------|-------------|
| 🚫 **Custom Blocklist** | Add any domain to block — supports exact and wildcard matching |
| 🔄 **Global On/Off** | Toggle all blocking on or off instantly |
| ⏱️ **5-Min Bypass** | Temporarily access a blocked site for 5 minutes, auto-reblocks |
| 💾 **Sync Storage** | Blocklist syncs across your Chrome devices |
| 🛡️ **MV3 Native** | Uses declarativeNetRequest — no legacy APIs, store-friendly |
| 🌐 **Auto Language** | Detects browser language, defaults to English |

---

## Supported Browsers

| Browser | Status |
|---------|--------|
| Google Chrome | ✅ Fully supported |
| Microsoft Edge | ✅ Fully supported |
| Other Chromium-based browsers | ✅ Should work |

---

## Installation

### From Source (Developer Mode)

1. Clone or download this repository
2. Open your browser's extension page:
   - **Chrome**: `chrome://extensions/`
   - **Edge**: `edge://extensions/`
3. Enable **Developer mode** (top-right toggle)
4. Click **Load unpacked** and select the `just-focus` folder
5. Click the 🎯 JustFocus icon in your toolbar to start

### Build (Minified + Zipped)

```bash
npm install
npm run build
```

Output: `dist/` folder + `just-focus-v1.0.0.zip` ready for Chrome Web Store upload.

---

## Usage

### Block a Website

1. Click the JustFocus icon in your toolbar
2. Type a domain (e.g. `youtube.com`) in the input field
3. Press Enter or click **+**
4. Done — visiting that site now redirects to a focus reminder page

### Temporarily Bypass

1. When you land on a blocked page, click **"Bypass 5 min"**
2. You'll be redirected to the site immediately
3. After 5 minutes, blocking resumes automatically

### Pause All Blocking

- Toggle the switch in the popup header to OFF
- All sites are unblocked instantly
- Toggle back ON to re-enable

---

## Privacy

- **declarativeNetRequest** — Blocks sites using declarative rules. Does not read page content.
- **storage** — Saves your blocklist locally. No data uploaded.
- **alarms** — Manages temp bypass timers. No background tracking.
- **activeTab** — Only accesses the current tab when you interact with the extension.
- Uses `<all_urls>` host permission only for declarativeNetRequest blocking rules. No tracking. No analytics. No external connections.

**[📄 Full Privacy Policy](privacy-policy.html)**

---

## Project Structure

```
just-focus/
├── manifest.json          # MV3 manifest
├── background.js          # Service worker (blocking logic)
├── blocked.html           # Block page with temp bypass
├── rules.json             # Dynamic rules (empty by default)
├── popup/
│   ├── popup.html         # Popup UI
│   ├── popup.css          # Styles (dark mode support)
│   └── popup.js           # Popup logic
├── icons/                 # Extension icons (on/off states)
├── assets/                # Support icons
├── images/                # Screenshots & promo images
├── _locales/              # i18n (en/zh_CN/ja/de/es/fr)
├── scripts/
│   └── build.js           # Build script (minify + zip)
├── languages/             # Multi-language READMEs
├── privacy-policy.html    # Privacy policy (6-language auto-detect)
├── support.html           # Support page
├── promo.html             # 1400×560 promotional tile template
└── store-listing.txt      # Chrome Web Store submission guide
```

---

## Copyright Disclaimer

This extension only blocks user-specified websites locally to help users maintain focus during work or study. The extension does not modify, copy, or redistribute any website content. All website content rights belong to their original publishers.

## License

Copyright © 2026 JustFocus. All rights reserved.

---

> **Note:** This repository is for **project showcase purposes only**. It does not contain the full source code, manifest, icons, or build scripts. Full source code will **not** be published here.
