# JustFocus

English | [中文](languages/README_zh.md) | [日本語](languages/README_ja.md) | [Deutsch](languages/README_de.md) | [Español](languages/README_es.md) | [Français](languages/README_fr.md)

A lightweight browser extension that blocks distracting websites to help you stay focused. Minimal, fast, and privacy-first.

> Chromium-based · Manifest V3 · Minimal Permissions · Local-First · No Tracking

---

## Why JustFocus?

Most site blockers are bloated with ads, forced sign-ups, and invasive tracking. JustFocus is different — it does one thing and does it well: **block the sites that distract you**.

| Advantage | Detail |
|-----------|--------|
| 🎯 **Single Purpose** | Block distracting sites. That's it. No bloat. |
| 🔒 **No Tracking** | No analytics, no accounts. Free tier is fully local — data never leaves your device |
| ⚡ **Lightweight** | Tiny footprint, no frameworks, no dependencies. |
| 🕐 **Temp Bypass** | Need 5 minutes? Bypass a site temporarily without removing it |
| 🔑 **Optional Password Lock** | Require a password to unblock — no more impulse visits |
| 🔄 **Global Toggle** | Pause all blocking with one switch — lunch break, weekends |
| 🌍 **6 Languages** | English, Chinese, Japanese, German, Spanish, French |

---

## Features

| Feature | Description |
|---------|-------------|
| 🚫 **Custom Blocklist** | Add any domain — all its subdomains are blocked automatically |
| 🔄 **Global On/Off** | Toggle all blocking on or off instantly |
| ⏱️ **5-Min Bypass** | Temporarily access a blocked site for 5 minutes, auto-reblocks |
| 💾 **Sync Storage** | Blocklist syncs across your Chrome devices |
| 🛡️ **MV3 Native** | Uses declarativeNetRequest — no legacy APIs, store-friendly |
| 🌐 **Auto Language** | Detects browser language, defaults to English |
| 📋 **Full List Page** | Manage every blocked site, edit durations, export & import |
| 🔑 **Password Protection** | Optional local password: unblocking, removing sites, and disabling blocking require it. Forgotten passwords cannot be recovered |
| ⭐ **Premium** | Surgical Blocking — hide Shorts / Reels / For You feeds while the rest of the site keeps working |

---

## Free vs Premium

| Capability | Free | Premium |
|------------|------|---------|
| Blocked sites (whole-site blocking) | **Unlimited** | Unlimited |
| Timed blocks (30 min → 24 h → permanent) | ✅ | ✅ |
| Global on/off toggle | ✅ | ✅ |
| 5-minute bypass | ✅ | ✅ |
| Optional password lock | ✅ | ✅ |
| Sync across Chrome devices | ✅ | ✅ |
| Export / import blocklist | ✅ | ✅ |
| Surgical Blocking — entry point | YouTube Shorts | All 12 sites |

**Everything except Surgical Blocking is free, with no site limit, no account and no sign-up.** Premium unlocks **Surgical Blocking** on the remaining sites.

| Site | What gets hidden | Free / Premium |
|------|------------------|----------------|
| YouTube | Shorts shelf, Shorts nav, `/shorts/` URLs | **Free** |
| Instagram | Reels tab and Reels feed | Premium |
| TikTok | For You feed | Premium |
| Facebook | Reels | Premium |
| Reddit | r/popular | Premium |
| Snapchat | Spotlight | Premium |
| VK | Clips | Premium |
| Pinterest | Home feed pins | Premium |
| Threads | For You feed (keeps Following) | Premium |
| LinkedIn | Home feed posts | Premium |
| X / Twitter | For You timeline (keeps Following) | Premium |
| Xiaohongshu | Explore feed | Premium |

> YouTube Shorts blocking is free for everyone — it is the single most requested case. Everything else under Surgical Blocking needs a Premium license.

- 🛒 Get a license: `https://www.annmax1983.com/checkout.html?plugin=justfocus`
- ⚙ Activate it: open the JustFocus popup → click the **⚙ / 🔒** button → enter your license key.

> License activation is **optional**. The free tier works fully without it — no account, no sign-up, no license key required.

---

## Supported Browsers

| Platform | Browser | Status |
|----------|---------|--------|
| Desktop | Google Chrome | ✅ Fully supported |
| Desktop | Microsoft Edge | ✅ Fully supported |
| Desktop | Other Chromium-based browsers (Brave, Vivaldi, Opera, Chromium) | ✅ Should work |
| Android | **Chrome for Android** | ❌ Not possible — Chrome for Android has no extension support at all |
| Android | Microsoft Edge Canary | ⚠️ Experimental extension support, limited catalog, unstable |
| Android | Chromium forks that load Chrome Web Store extensions (e.g. Quetta, Yandex) | ⚠️ Unofficial; should work but untested |
| Android | Firefox for Android | ❌ Not available — JustFocus is built on Chromium MV3 (`declarativeNetRequest`) and is not published on AMO |
| iOS | Any | ❌ Not possible — no browser on iOS supports extensions outside of Safari |

> **Short version:** this is a desktop browser extension. Installing it on a phone is not supported — Chrome for Android does not accept extensions, and the workarounds (Edge Canary, third-party Chromium forks) are experimental and not something we can support. Blocking works on desktop Chrome and Edge.

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

Output: `dist/` folder + `publish/just-focus-v<version>.zip` ready for Chrome Web Store upload.

> The build strips console noise, minifies the JS and refuses to ship anything from `images/` (store screenshots) — the zip is checked after it is built, not assumed to be clean.

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

### Password Protection (Optional)

Don't trust yourself with the bypass button? Set a password:

1. Open the popup → click **⚙ / 🔒** → *Password Protection* section, or the 🔒 button on the list page
2. Set a password (min. 4 characters) — it is stored **only on this device** as a salted hash, never uploaded
3. From then on, these actions require the password:
   - Turning blocking off (global switch)
   - 5-minute bypass on the block page
   - Removing a site or clearing the list
   - Editing a block duration
4. Change or remove the password anytime (the current password is required)

> ⚠️ **Forgotten passwords cannot be recovered.** There is no reset link, no recovery, no backdoor — by design. Choose something you will actually remember.

---

## Privacy

- **declarativeNetRequest** — Blocks sites using declarative rules. Does not read page content.
- **storage** — Saves your blocklist locally. No data uploaded.
- **Password (optional)** — If you set a password, only a salted hash is stored in local device storage. It never syncs and is never uploaded. Forgotten passwords cannot be recovered.
- **alarms** — Manages temp bypass timers. No background tracking.
- **activeTab** — Only accesses the current tab when you interact with the extension.
- **License (optional)** — Only if you activate a paid license: a random install identifier + browser metadata is sent to `api.annmax1983.com` to activate/validate the license. This never includes your blocklist, browsing history, or personal data.
- Uses `<all_urls>` host permission only for declarativeNetRequest blocking rules, and the license server only for paid activation. No tracking. No analytics. Free users' data never leaves the device.

**[📄 Full Privacy Policy](privacy-policy.html)**

---

## Copyright Disclaimer

This extension only blocks user-specified websites locally to help users maintain focus during work or study. The extension does not modify, copy, or redistribute any website content. All website content rights belong to their original publishers.

## License

Copyright © 2026 JustFocus. All rights reserved.

---

> **Note:** the official installation channel is the Chrome Web Store. This repository carries the extension's own documentation and source for reference — it is not a distribution channel and no offline/unsigned package is published here.
