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
| 🔑 **Passwortschutz** | Optionales lokales Passwort: Entsperren, Seiten entfernen und Blockierung deaktivieren erfordern es. Vergessene Passwörter sind nicht wiederherstellbar |
| ⭐ **Premium** | Chirurgisches Blockieren — nur Shorts, Reels und For-You-Feeds ausblenden, der Rest der Seite bleibt nutzbar (einmalige VKT Premium-Lizenz) |

---

## Kostenlos vs. Premium

| Plan | Blockierte Seiten | Export / Import | Chirurgisches Blockieren |
|------|-------------------|-----------------|--------------------------|
| **Kostenlos** | Unbegrenzt | Inklusive | Nur YouTube Shorts |
| **⭐ Premium** | Unbegrenzt | Inklusive | Alle 12 unterstützten Seiten |

Das Blockieren ablenkender Seiten ist **komplett kostenlos, ohne Seitenlimit**. **Premium schaltet chirurgisches Blockieren frei** — nur die süchtig machenden Teile ausblenden (Shorts, Reels, For-You-Feeds), der Rest der Seite bleibt nutzbar — auf YouTube, Instagram, TikTok, Facebook, Reddit, X, Pinterest, Threads, LinkedIn, Snapchat, VK und Xiaohongshu.

> Das Blockieren von YouTube Shorts ist für alle kostenlos, alle anderen Seiten erfordern eine Premium-Lizenz.

- 🛒 Lizenz erhalten: `https://www.annmax1983.com/checkout.html?plugin=justfocus`
- ⚙ Aktivieren: JustFocus Popup öffnen → **⚙ / 🔒**-Button klicken → Lizenzschlüssel eingeben.

> Die Lizenzaktivierung ist **optional**. Die kostenlose Stufe funktioniert vollständig ohne sie — kein Konto, keine Anmeldung, kein Lizenzschlüssel erforderlich.

---

## Unterstützte Browser

| Plattform | Browser | Status |
|---------|--------|--------|
| Desktop | Google Chrome | ✅ Vollständig unterstützt |
| Desktop | Microsoft Edge | ✅ Vollständig unterstützt |
| Desktop | Andere Chromium-basierte Browser (Brave, Vivaldi, Opera, Chromium) | ✅ Sollte funktionieren |
| Android | **Chrome für Android** | ❌ Nicht möglich — Chrome für Android unterstützt keinerlei Erweiterungen |
| Android | Microsoft Edge Canary | ⚠️ Experimentelle Erweiterungsunterstützung, kleiner Katalog, instabil |
| Android | Chromium-Forks, die Chrome-Web-Store-Erweiterungen laden (z. B. Quetta, Yandex) | ⚠️ Inoffiziell; sollte funktionieren, aber ungetestet |
| Android | Firefox für Android | ❌ Nicht verfügbar — JustFocus basiert auf Chromium MV3 (`declarativeNetRequest`) und ist nicht auf AMO veröffentlicht |
| iOS | Alle | ❌ Nicht möglich — kein Browser unter iOS unterstützt Erweiterungen außerhalb von Safari |

> **Kurz gesagt:** Dies ist eine Desktop-Browser-Erweiterung. Die Installation auf einem Smartphone wird nicht unterstützt — Chrome für Android akzeptiert keine Erweiterungen, und die Workarounds (Edge Canary, Chromium-Forks Dritter) sind experimentell. Das Blockieren funktioniert unter Chrome und Edge für Desktop.

---

## Installation

| Store | Link |
|---|---|
| Chrome Web Store | [In Chrome installieren](https://chromewebstore.google.com/detail/iocnhglbdkdonajhkipknhgdnbombcic) |
| Microsoft Edge Add-ons | [In Edge installieren](https://microsoftedge.microsoft.com/addons/detail/eigeengnoahojmfcnkkjnipbdnpngaod) |

> Installieren Sie nur über die offiziellen Stores oben – meiden Sie Download-Seiten Dritter.

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

### Passwortschutz (optional)

Traust du dem Umgehungs-Button nicht? Setze ein Passwort:

1. Popup öffnen → **⚙ / 🔒** → Abschnitt *Passwortschutz*, oder den 🔒-Button auf der Listen-Seite
2. Passwort festlegen (min. 4 Zeichen) — es wird nur als gesalzener Hash **auf diesem Gerät** gespeichert, nie hochgeladen
3. Fortan erfordern diese Aktionen das Passwort:
   - Blockierung ausschalten (globaler Schalter)
   - 5-Min-Umgehung auf der Blockierseite
   - Seite entfernen oder Liste leeren
   - Blockierdauer bearbeiten
4. Passwort jederzeit ändern oder entfernen (aktuelles Passwort erforderlich)

> ⚠️ **Vergessene Passwörter können nicht wiederhergestellt werden.** Kein Reset-Link, keine Wiederherstellung, kein Backdoor — by Design. Wähle etwas, das du dir wirklich merkst.

---

## Datenschutz

- **declarativeNetRequest** — Blockiert Seiten mit Hilfe von deklarativen Regeln. Liest keinen Seiteninhalt.
- **storage** — Speichert deine Blockliste lokal. Keine Daten hochgeladen.
- **Passwort (optional)** — Bei Aktivierung wird nur ein gesalzener Hash lokal gespeichert. Keine Synchronisation, kein Upload. Vergessene Passwörter sind nicht wiederherstellbar.
- **alarms** — Verwaltet temporäre Umgehungs-Timer. Kein Hintergrund-Tracking.
- **activeTab** — Greift nur auf den aktuellen Tab zu, wenn du mit der Erweiterung interagierst.
- **Lizenz (optional)** — Nur bei Aktivierung einer kostenpflichtigen Lizenz: Lizenzschlüssel und eine zufällige Installationskennung + Browser-Metadaten werden an `api.annmax1983.com` gesendet, um die Lizenz zu aktivieren/validieren. Dies enthält nie deine Blockliste, deinen Browserverlauf oder persönliche Daten.
- Verwendet `<all_urls>` Host-Berechtigung nur für declarativeNetRequest-Blockierregeln, und den Lizenzserver nur für kostenpflichtige Aktivierung. Kein Tracking. Keine Analytik. Daten von kostenlosen Nutzern verlassen nie das Gerät.

**[📄 Vollständige Datenschutzerklärung](privacy-policy.html)**

---

## Urheberrechtshinweis

Diese Erweiterung blockiert nur benutzerdefinierte Websites lokal, um Nutzern zu helfen, während der Arbeit oder beim Lernen konzentriert zu bleiben. Die Erweiterung verändert, kopiert oder verbreitet keinen Website-Inhalt. Alle Website-Inhaltsrechte gehören deren jeweiligen Herausgebern.

## Lizenz

Copyright © 2026 JustFocus. Alle Rechte vorbehalten.

---

> **Hinweis:** Der offizielle Installationsweg ist der Chrome Web Store. Dieses Repository enthält die Dokumentation und den Quellcode der Erweiterung als Referenz — es ist kein Vertriebsweg, und es werden hier keine Offline- oder unsignierten Pakete veröffentlicht.
