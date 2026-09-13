# JustFocus

[English](../README.md) | [中文](README_zh.md) | [日本語](README_ja.md) | Deutsch | [Español](README_es.md) | [Français](README_fr.md)

Eine schlanke Browser-Erweiterung, die ablenkende Websites blockiert, damit du konzentriert bleibst. Minimalistisch, schnell und mit Fokus auf Datenschutz.

> Chromium-basiert · Manifest V3 · Minimale Berechtigungen · Lokal zuerst · Kein Tracking

---

## Warum JustFocus?

Die meisten Seiten-Blocker sind voller Werbung, erzwungener Anmeldungen und invasiven Trackings. JustFocus ist anders — es macht eine Sache und macht sie gut: **Die Seiten blockieren, die dich ablenken**.

| Vorteil | Details |
|---------|---------|
| 🎯 **Einzelzweck** | Ablenkende Seiten blockieren. Das ist alles. Kein Ballast. |
| 🔒 **Kein Tracking** | Keine Analytik, keine Konten. Die kostenlose Stufe ist komplett lokal — Daten verlassen nie dein Gerät |
| ⚡ **Leichtgewichtig** | Winziger Fußabdruck, keine Frameworks, keine Abhängigkeiten. |
| 🕐 **Temporär umgehen** | 5 Minuten nötig? Seite temporär umgehen ohne sie zu entfernen |
| 🔄 **Globaler Schalter** | Gesamte Blockierung mit einem Schalter pausieren — Mittagspause, Wochenende |
| 🌍 **6 Sprachen** | Englisch, Chinesisch, Japanisch, Deutsch, Spanisch, Französisch |

---

## Funktionen

| Funktion | Beschreibung |
|----------|--------------|
| 🚫 **Eigene Blockliste** | Beliebige Domain hinzufügen — alle ihre Subdomains werden automatisch blockiert |
| 🔄 **Global EIN/AUS** | Gesamte Blockierung sofort ein- oder ausschalten |
| ⏱️ **5-Min Umgehung** | Auf eine blockierte Seite für 5 Minuten zugreifen, wird automatisch wieder blockiert |
| 💾 **Sync-Speicher** | Blockliste wird über deine Chrome-Geräte hinweg synchronisiert |
| 🛡️ **MV3 nativ** | Verwendet declarativeNetRequest — keine Legacy-APIs, Store-freundlich |
| 🌐 **Auto-Sprache** | Erkennt Browsersprache, Standard ist Englisch |
| 📋 **Vollständige Listen-Seite** | Jede blockierte Seite verwalten, Dauern bearbeiten, Exportieren & Importieren |
| ⭐ **Premium** | Unbegrenzte Seiten + Export/Import mit einer einmaligen VKT Premium-Lizenz |

---

## Kostenlos vs. Premium

| Plan | Blockierte Seiten | Export / Import |
|------|-------------------|-----------------|
| **Kostenlos** | Bis zu 10 aktive Seiten | — |
| **⭐ Premium** | Unbegrenzt | ✅ Inklusive |

JustFocus ist kostenlos für bis zu **10 aktive blockierte Seiten**. Für unbegrenzte Seiten plus **Export / Import** deiner Blockliste, aktiviere eine **VKT Premium** Lizenz — ein einmaliger Kauf, der die Entwicklung unterstützt.

- 🛒 Lizenz erhalten: `https://www.annmax1983.com/checkout.html?plugin=justfocus`
- ⚙ Aktivieren: JustFocus Popup öffnen → **⚙ / 🔒**-Button klicken → Lizenzschlüssel eingeben.

> Die Lizenzaktivierung ist **optional**. Die kostenlose Stufe funktioniert vollständig ohne sie — kein Konto, keine Anmeldung, kein Lizenzschlüssel erforderlich.

---

## Unterstützte Browser

| Browser | Status |
|---------|--------|
| Google Chrome | ✅ Vollständig unterstützt |
| Microsoft Edge | ✅ Vollständig unterstützt |
| Andere Chromium-basierte Browser | ✅ Sollte funktionieren |

---

## Installation

### Aus dem Quellcode (Entwicklermodus)

1. Repository klonen oder herunterladen
2. Öffne die Erweiterungsseite deines Browsers:
   - **Chrome**: `chrome://extensions/`
   - **Edge**: `edge://extensions/`
3. Aktiviere den **Entwicklermodus** (Schalter oben rechts)
4. Klicke auf **Entpackte Erweiterung laden** und wähle den Ordner `just-focus`
5. Klicke auf das 🎯 JustFocus-Symbol in deiner Toolbar zum Starten

### Build (Minifiziert + Gezippt)

```bash
npm install
npm run build
```

Output: `dist/`-Ordner + `just-focus-v1.0.0.zip` bereit für den Chrome Web Store Upload.

---

## Verwendung

### Eine Website blockieren

1. Klicke auf das JustFocus-Symbol in deiner Toolbar
2. Gib eine Domain ein (z.B. `youtube.com`) im Eingabefeld
3. Drücke Enter oder klicke auf **+**
4. Fertig — der Besuch dieser Seite leitet jetzt auf eine Fokus-Erinnerungsseite um

### Temporär umgehen

1. Wenn du auf einer blockierten Seite landest, klicke auf **„5 Min umgehen"**
2. Du wirst sofort zur Seite weitergeleitet
3. Nach 5 Minuten wird die Blockierung automatisch wieder aktiviert

### Gesamte Blockierung pausieren

- Schalte den Schalter im Popup-Header auf AUS
- Alle Seiten werden sofort entsperrt
- Zurück auf EIN schalten, um erneut zu aktivieren

---

## Datenschutz

- **declarativeNetRequest** — Blockiert Seiten mit Hilfe von deklarativen Regeln. Liest keinen Seiteninhalt.
- **storage** — Speichert deine Blockliste lokal. Keine Daten hochgeladen.
- **alarms** — Verwaltet temporäre Umgehungs-Timer. Kein Hintergrund-Tracking.
- **activeTab** — Greift nur auf den aktuellen Tab zu, wenn du mit der Erweiterung interagierst.
- **Lizenz (optional)** — Nur bei Aktivierung einer kostenpflichtigen Lizenz: Ein Geräte-Fingerprint + Browser-Metadaten werden an `api.annmax1983.com` gesendet, um die Lizenz zu aktivieren/validieren. Dies enthält nie deine Blockliste, deinen Browserverlauf oder persönliche Daten.
- Verwendet `<all_urls>` Host-Berechtigung nur für declarativeNetRequest-Blockierregeln, und den Lizenzserver nur für kostenpflichtige Aktivierung. Kein Tracking. Keine Analytik. Daten von kostenlosen Nutzern verlassen nie das Gerät.

**[📄 Vollständige Datenschutzerklärung](privacy-policy.html)**

---

## Projektstruktur

```
just-focus/
├── manifest.json          # MV3 Manifest
├── background.js          # Service Worker (Blockierlogik)
├── license.js             # Lizenzmanager (Aktivierung & Validierung)
├── blocked.html           # Blockierseite mit temporärer Umgehung
├── popup/
│   ├── popup.html         # Popup-UI (Zusammenfassung + Lizenzmodal)
│   ├── popup.css          # Styles (Dark Mode Support)
│   └── popup.js           # Popup-Logik
├── list/
│   ├── list.html          # Vollständige Listen-Manager-Seite
│   ├── list.css           # Styles
│   └── list.js            # Vollständige Liste + Export/Import-Logik
├── icons/                 # Erweiterungs-Symbole (Ein/Aus-Zustände)
├── assets/                # Support-Symbole
├── images/                # Screenshots & Promo-Bilder
├── _locales/              # i18n (en/zh_CN/ja/de/es/fr)
├── scripts/
│   └── build.js           # Build-Skript (Minifizieren + Zippen)
├── languages/             # Mehrsprachige READMEs
├── privacy-policy.html    # Datenschutzerklärung (6-Sprachen Auto-Erkennung)
├── support.html           # Support-Seite
├── promo.html             # 1400×560 Promo-Tile-Vorlage
└── store-listing.txt      # Chrome Web Store Einreichungsleitfaden
```

---

## Urheberrechtshinweis

Diese Erweiterung blockiert nur benutzerdefinierte Websites lokal, um Nutzern zu helfen, während der Arbeit oder beim Lernen konzentriert zu bleiben. Die Erweiterung verändert, kopiert oder verbreitet keinen Website-Inhalt. Alle Website-Inhaltsrechte gehören deren jeweiligen Herausgebern.

## Lizenz

Copyright © 2026 JustFocus. Alle Rechte vorbehalten.

---

> **Hinweis:** Dieses Repository dient ausschließlich der **Projektpräsentation**. Es enthält nicht den vollständigen Quellcode, das Manifest, Icons oder Build-Skripte. Der vollständige Quellcode wird hier **nicht** veröffentlicht.
