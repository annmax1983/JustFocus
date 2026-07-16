# JustFocus

[English](../README.md) | [中文](README_zh.md) | [日本語](README_ja.md) | [Deutsch](README_de.md) | [Español](README_es.md) | Français

Une extension de navigateur légère qui bloque les sites distrayants pour vous aider à rester concentré. Minimal, rapide et axé sur la confidentialité.

> Basée sur Chromium · Manifest V3 · Permissions minimales · Entièrement local · Aucun suivi

---

## Pourquoi JustFocus ?

La plupart des bloqueurs de sites sont gonflés de publicités, d'inscriptions forcées et de traçage invasif. JustFocus est différent — il fait une chose et la fait bien : **bloquer les sites qui vous distraient**.

| Avantage | Détail |
|----------|--------|
| 🎯 **Objectif unique** | Bloquer les sites distrayants. C'est tout. Sans surcharge. |
| 🔒 **Aucun suivi** | Pas d'analytics, pas de comptes, aucune collecte de données |
| ⚡ **Léger** | Moins de 50KB au total. Pas de frameworks, pas de dépendances. |
| 🕐 **Contournement temporaire** | Besoin de 5 minutes ? Accédez temporairement sans le supprimer |
| 🔄 **Interrupteur global** | Mettez en pause tout le blocage avec un interrupteur |
| 🌍 **6 langues** | Anglais, chinois, japonais, allemand, espagnol, français |

---

## Fonctionnalités

| Fonctionnalité | Description |
|----------------|-------------|
| 🚫 **Liste noire personnalisée** | Ajoutez n'importe quel domaine — correspondance exacte et générique |
| 🔄 **Global On/Off** | Activez ou désactivez tout le blocage instantanément |
| ⏱️ **Contournement 5 min** | Accédez à un site bloqué pendant 5 minutes, re-blocage automatique |
| 💾 **Stockage sync** | La liste se synchronise entre vos appareils Chrome |
| 🛡️ **MV3 natif** | Utilise declarativeNetRequest — pas d'APIs legacy |
| 🌐 **Langue automatique** | Détecte la langue du navigateur, anglais par défaut |

---

## Installation

### Depuis le code source (Mode développeur)

1. Cloner ou télécharger le dépôt
2. Ouvrir la page des extensions :
   - **Chrome** : `chrome://extensions/`
   - **Edge** : `edge://extensions/`
3. Activer le **Mode développeur**
4. Cliquer sur **Charger l'extension non empaquetée** et sélectionner le dossier `just-focus`
5. Cliquer sur l'icône 🎯 JustFocus dans la barre d'outils

### Build (Minifié + Zip)

```bash
npm install
npm run build
```

Sortie : dossier `dist/` + `just-focus-v1.0.0.zip`

---

## Utilisation

### Bloquer un site

1. Cliquer sur l'icône JustFocus
2. Taper un domaine (ex : `youtube.com`)
3. Appuyer sur Entrée ou cliquer sur **+**
4. Terminé — la visite de ce site redirige vers une page de rappel de concentration

### Contournement temporaire

1. Sur la page bloquée, cliquer sur **"Contourner 5 min"**
2. Redirection immédiate vers le site
3. Après 5 minutes, le blocage reprend automatiquement

---

## Confidentialité

- **declarativeNetRequest** — Bloque les sites avec des règles déclaratives. Ne lit pas le contenu des pages.
- **storage** — Enregistre la liste localement. Aucune donnée uploadée.
- **alarms** — Gère les minuteurs de contournement. Pas de suivi en arrière-plan.
- **activeTab** — Accès uniquement lors d'une interaction active.
- Pas de permission hôte `<all_urls>`. Pas de suivi. Pas d'analytics. Pas de connexions externes.

**[📄 Politique de Confidentialité](../privacy-policy.html)**

---

## Licence

Copyright © 2026 JustFocus. Tous droits réservés.

---

> **Note :** Ce dépôt est uniquement pour la **présentation du projet**.
