# JustFocus

[English](../README.md) | [中文](README_zh.md) | [日本語](README_ja.md) | Deutsch | [Español](README_es.md) | [Français](README_fr.md)

Eine leichtgewichtige Browser-Erweiterung, die ablenkende Websites blockiert, um Ihnen zu helfen, fokussiert zu bleiben. Minimal, schnell und datenschutzfreundlich.

> Chromium-basiert · Manifest V3 · Minimale Berechtigungen · Vollständig lokal · Kein Tracking

---

## Warum JustFocus?

Die meisten Website-Blocker sind mit Werbung, erzwungenen Anmeldungen und invasivem Tracking überladen. JustFocus ist anders — es macht eine Sache und macht sie gut: **Ablenkende Websites blockieren**.

| Vorteil | Detail |
|---------|--------|
| 🎯 **Einziger Zweck** | Ablenkende Seiten blockieren. Mehr nicht. Kein Ballast. |
| 🔒 **Kein Tracking** | Keine Analysen, keine Konten, keinerlei Datenerfassung |
| ⚡ **Leichtgewichtig** | Unter 50KB gesamt. Keine Frameworks, keine Abhängigkeiten. |
| 🕐 **Temporäre Umgehung** | 5 Minuten nötig? Seite temporär freigeben ohne sie zu entfernen |
| 🔄 **Globaler Schalter** | Alle Blockierungen mit einem Schalter pausieren |
| 🌍 **6 Sprachen** | Englisch, Chinesisch, Japanisch, Deutsch, Spanisch, Französisch |

---

## Funktionen

| Funktion | Beschreibung |
|----------|-------------|
| 🚫 **Benutzerdefinierte Sperrliste** | Beliebige Domains hinzufügen — exakte und Wildcard-Erkennung |
| 🔄 **Global An/Aus** | Alle Blockierungen sofort umschalten |
| ⏱️ **5-Min Umgehung** | Gesperrte Seite für 5 Minuten freigeben, automatische Wiedersperrung |
| 💾 **Synchronisation** | Sperrliste synchronisiert sich über Chrome-Geräte |
| 🛡️ **MV3 nativ** | Verwendet declarativeNetRequest — keine Legacy-APIs |
| 🌐 **Automatische Sprache** | Erkennt Browsersprache, Standard ist Englisch |

---

## Installation

### Aus dem Quellcode (Entwicklermodus)

1. Repository klonen oder herunterladen
2. Browser-Erweiterungsseite öffnen:
   - **Chrome**: `chrome://extensions/`
   - **Edge**: `edge://extensions/`
3. **Entwicklermodus** aktivieren
4. **Entpackte Erweiterung laden** klicken und `just-focus`-Ordner auswählen
5. 🎯 JustFocus-Symbol in der Symbolleiste klicken

### Build (Minifiziert + Zip)

```bash
npm install
npm run build
```

Ausgabe: `dist/` Ordner + `just-focus-v1.0.0.zip`

---

## Verwendung

### Website sperren

1. JustFocus-Symbol klicken
2. Domain eingeben (z.B. `youtube.com`)
3. Enter drücken oder **+** klicken
4. Fertig — Besuch der Seite leitet zur Fokuserinnerung weiter

### Temporär umgehen

1. Auf der Sperrseite **"5 Min umgehen"** klicken
2. Sofortige Weiterleitung zur Website
3. Nach 5 Minuten wird die Sperrung automatisch wiederhergestellt

---

## Datenschutz

- **declarativeNetRequest** — Blockiert Websites mit deklarativen Regeln. Liest keine Seiteninhalte.
- **storage** — Speichert Sperrliste lokal. Keine Daten hochgeladen.
- **alarms** — Verwaltet temporäre Umgehungstimer. Kein Hintergrund-Tracking.
- **activeTab** — Nur Zugriff bei aktiver Interaktion mit der Erweiterung.
- Keine `<all_urls>` Host-Berechtigung. Kein Tracking. Keine Analysen. Keine externen Verbindungen.

**[📄 Datenschutzrichtlinie](../privacy-policy.html)**

---

## Lizenz

Copyright © 2026 JustFocus. Alle Rechte vorbehalten.

---

> **Hinweis:** Dieses Repository dient nur zur **Projektpräsentation**.
