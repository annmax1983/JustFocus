# JustFocus

[English](../README.md) | [中文](README_zh.md) | [日本語](README_ja.md) | [Deutsch](README_de.md) | [Español](README_es.md) | Français

Une extension légère qui bloque les sites web distrayants pour vous aider à rester concentré. Minimal, rapide et respectueux de votre vie privée.

> Chromium · Manifest V3 · Permissions minimales · Local d'abord · Aucun suivi

---

## Pourquoi JustFocus ?

La plupart des bloqueurs de sites sont gonflés de publicités, d'inscriptions obligatoires et de traqueurs invasifs. JustFocus est différent — il fait une seule chose et la fait bien : **bloquer les sites qui vous distraient**.

| Avantage | Détail |
|-----------|--------|
| 🎯 **Objectif unique** | Bloquer les sites distrayants. C'est tout. Pas de superflu. |
| 🔒 **Pas de suivi** | Pas d'analytics, pas de comptes. Le niveau gratuit est entièrement local — vos données ne quittent jamais votre appareil |
| ⚡ **Léger** | Empreinte minuscule, pas de frameworks, pas de dépendances |
| 🕐 **Contournement temporaire** | Besoin de 5 minutes ? Contournez un site temporairement sans le retirer |
| 🔄 **Activation globale** | Mettez en pause tout le blocage avec un seul interrupteur — pause déjeuner, week-end |
| 🌍 **6 langues** | English, 中文, 日本語, Deutsch, Español, Français |

---

## Fonctionnalités

| Fonctionnalité | Description |
|---------|-------------|
| 🚫 **Liste de blocage personnalisée** | Ajoutez n'importe quel domaine — tous ses sous-domaines sont bloqués automatiquement |
| 🔄 **Activation/Désactivation globale** | Activez ou désactivez tout le blocage instantanément |
| ⏱️ **Contournement 5 min** | Accédez temporairement à un site bloqué pendant 5 minutes, rebloquage automatique |
| 💾 **Synchronisation** | La liste de blocage se synchronise sur vos appareils Chrome |
| 🛡️ **Natif MV3** | Utilise `declarativeNetRequest` — aucune API obsolète, compatible avec la boutique |
| 🌐 **Langue automatique** | Détecte la langue du navigateur, anglais par défaut |
| 📋 **Page de liste complète** | Gérez chaque site bloqué, modifiez les durées, exportez et importez |
| ⭐ **Premium** | Sites illimités + Export/Import avec une licence VKT Premium unique |

---

## Gratuit vs Premium

| Plan | Sites bloqués | Export / Import |
|------|---------------|-----------------|
| **Gratuit** | Jusqu'à 10 sites actifs | — |
| **⭐ Premium** | Illimité | ✅ Inclus |

JustFocus est gratuit pour jusqu'à **10 sites bloqués actifs**. Pour un nombre illimité de sites et l'**Export / Import** de votre liste de blocage, activez une licence **VKT Premium** — un achat unique qui soutient le développement.

- 🛒 Obtenir une licence : `https://www.annmax1983.com/checkout.html?plugin=justfocus`
- ⚙ L'activer : ouvrez le popup JustFocus → cliquez sur le bouton **⚙ / 🔒** → saisissez votre clé de licence.

> L'activation de la licence est **optionnelle**. Le niveau gratuit fonctionne entièrement sans elle — pas de compte, pas d'inscription, pas de clé de licence requise.

---

## Navigateurs compatibles

| Navigateur | Statut |
|---------|--------|
| Google Chrome | ✅ Entièrement pris en charge |
| Microsoft Edge | ✅ Entièrement pris en charge |
| Autres navigateurs basés sur Chromium | ✅ Devrait fonctionner |

---

## Installation

### Depuis les sources (mode développeur)

1. Clonez ou téléchargez ce dépôt
2. Ouvrez la page des extensions de votre navigateur :
   - **Chrome** : `chrome://extensions/`
   - **Edge** : `edge://extensions/`
3. Activez le **mode Développeur** (bouton en haut à droite)
4. Cliquez sur **Charger le package décompressé** et sélectionnez le dossier `just-focus`
5. Cliquez sur l'icône 🎯 JustFocus dans votre barre d'outils pour commencer

### Build (Minifié + Zippé)

```bash
npm install
npm run build
```

Résultat : dossier `dist/` + `just-focus-v1.0.0.zip` prêt pour l'upload sur le Chrome Web Store.

---

## Utilisation

### Bloquer un site web

1. Cliquez sur l'icône JustFocus dans votre barre d'outils
2. Saisissez un domaine (ex. `youtube.com`) dans le champ de saisie
3. Appuyez sur Entrée ou cliquez sur **+**
4. C'est fait — la visite de ce site redirige maintenant vers une page de rappel de concentration

### Contournement temporaire

1. Quand vous atterrissez sur une page bloquée, cliquez sur **« Contourner 5 min »**
2. Vous êtes redirigé vers le site immédiatement
3. Après 5 minutes, le blocage reprend automatiquement

### Mettre en pause tout le blocage

- Basculez l'interrupteur dans l'en-tête du popup sur OFF
- Tous les sites sont débloqués instantanément
- Rebasculez sur ON pour réactiver

---

## Confidentialité

- **declarativeNetRequest** — Bloque les sites via des règles déclaratives. Ne lit pas le contenu des pages.
- **storage** — Sauvegarde votre liste de blocage en local. Aucune donnée envoyée.
- **alarms** — Gère les minuteurs de contournement temporaire. Aucun suivi en arrière-plan.
- **activeTab** — N'accède à l'onglet actif que lorsque vous interagissez avec l'extension.
- **Licence (optionnelle)** — Uniquement si vous activez une licence payante : une empreinte de l'appareil + des métadonnées du navigateur sont envoyées à `api.annmax1983.com` pour activer/valider la licence. Cela n'inclut jamais votre liste de blocage, votre historique de navigation ni vos données personnelles.
- Utilise la permission `<all_urls>` uniquement pour les règles de blocage `declarativeNetRequest`, et le serveur de licence uniquement pour l'activation payante. Aucun suivi. Aucun analytics. Les données des utilisateurs gratuits ne quittent jamais l'appareil.

**[📄 Politique de confidentialité complète](privacy-policy.html)**

---

## Structure du projet

```
just-focus/
├── manifest.json          # Manifest MV3
├── background.js          # Service worker (logique de blocage)
├── license.js             # Gestionnaire de licences (activation et validation)
├── blocked.html           # Page de blocage avec contournement temporaire
├── popup/
│   ├── popup.html         # Interface popup (résumé + modale de licence)
│   ├── popup.css          # Styles (support du mode sombre)
│   └── popup.js           # Logique du popup
├── list/
│   ├── list.html          # Page de gestion de la liste complète
│   ├── list.css           # Styles
│   └── list.js            # Logique liste complète + export/import
├── icons/                 # Icônes de l'extension (états on/off)
├── assets/                # Icônes de support
├── images/                # Captures d'écran et images promotionnelles
├── _locales/              # i18n (en/zh_CN/ja/de/es/fr)
├── scripts/
│   └── build.js           # Script de build (minification + zip)
├── languages/             # READMEs multilingues
├── privacy-policy.html    # Politique de confidentialité (détection automatique en 6 langues)
├── support.html           # Page de support
├── promo.html             # Modèle de tuile promotionnelle 1400×560
└── store-listing.txt      # Guide de soumission au Chrome Web Store
```

---

## Avertissement relatif au droit d'auteur

Cette extension bloque uniquement les sites web spécifiés par l'utilisateur en local pour l'aider à maintenir sa concentration pendant le travail ou les études. L'extension ne modifie, ne copie ni ne redistribue aucun contenu de site web. Tous les droits de contenu des sites appartiennent à leurs éditeurs originaux.

## Licence

Copyright © 2026 JustFocus. Tous droits réservés.

---

> **Note :** Ce dépôt est destiné à la **présentation du projet uniquement**. Il ne contient pas le code source complet, le manifest, les icônes ou les scripts de build. Le code source complet ne sera **pas** publié ici.
