# JustFocus

[English](../README.md) | [中文](README_zh.md) | [日本語](README_ja.md) | [Deutsch](README_de.md) | [Español](README_es.md) | Français

Une extension légère qui bloque les sites web distrayants pour vous aider à rester concentré. Minimal, rapide et respectueux de votre vie privée.

> Chrome / Edge / Firefox · Manifest V3 · Permissions minimales · Local d'abord · Aucun suivi

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
| 💾 **Synchronisation** | La liste de blocage se synchronise sur vos appareils (Chrome, Edge ou Firefox) |
| 🛡️ **Natif MV3** | Utilise `declarativeNetRequest` — aucune API obsolète, compatible avec la boutique |
| 🌐 **Langue automatique** | Détecte la langue du navigateur, anglais par défaut |
| 📋 **Page de liste complète** | Gérez chaque site bloqué, modifiez les durées, exportez et importez |
| 🔑 **Protection par mot de passe** | Mot de passe local optionnel : débloquer, supprimer des sites et désactiver le blocage le nécessitent. Un mot de passe oublié est irrécupérable |
| ⭐ **Premium** | Blocage chirurgical — masquez uniquement Shorts, Reels et Pour vous, le reste du site reste utilisable (licence VKT Premium unique) |

---

## Gratuit vs Premium

| Plan | Sites bloqués | Export / Import | Blocage chirurgical |
|------|---------------|-----------------|---------------------|
| **Gratuit** | Illimité | Inclus | YouTube Shorts uniquement |
| **⭐ Premium** | Illimité | Inclus | Les 12 sites pris en charge |

Bloquer les sites distrayants est **entièrement gratuit, sans limite de sites**. **Premium ajoute le blocage chirurgical** — masquez uniquement les parties addictives (Shorts, Reels, Pour vous), le reste du site reste utilisable — sur YouTube, Instagram, TikTok, Facebook, Reddit, X, Pinterest, Threads, LinkedIn, Snapchat, VK et Xiaohongshu.

> Le blocage de YouTube Shorts est gratuit pour tous, les autres sites nécessitent une licence Premium.

- 🛒 Obtenir une licence : `https://www.annmax1983.com/checkout.html?plugin=justfocus`
- ⚙ L'activer : ouvrez le popup JustFocus → cliquez sur le bouton **⚙ / 🔒** → saisissez votre clé de licence.

> L'activation de la licence est **optionnelle**. Le niveau gratuit fonctionne entièrement sans elle — pas de compte, pas d'inscription, pas de clé de licence requise.

---

## Navigateurs compatibles

| Plateforme | Navigateur | Statut |
|---------|--------|--------|
| Bureau | Google Chrome | ✅ Entièrement pris en charge |
| Bureau | Microsoft Edge | ✅ Entièrement pris en charge |
| Bureau | Autres navigateurs basés sur Chromium (Brave, Vivaldi, Opera, Chromium) | ✅ Devrait fonctionner |
| Android | **Chrome pour Android** | ❌ Impossible — Chrome pour Android ne prend en charge aucune extension |
| Android | Microsoft Edge Canary | ⚠️ Prise en charge expérimentale, catalogue limité, instable |
| Android | Forks Chromium qui chargent les extensions du Chrome Web Store (ex. Quetta, Yandex) | ⚠️ Non officiel ; devrait fonctionner mais non testé |
| Android | Firefox pour Android | ❌ Indisponible — JustFocus est bâti sur Chromium MV3 (`declarativeNetRequest`) et n'est pas publié sur AMO |
| iOS | Tous | ❌ Impossible — aucun navigateur sur iOS ne prend en charge les extensions en dehors de Safari |

> **En bref :** c'est une extension de navigateur de bureau. L'installation sur téléphone n'est pas prise en charge — Chrome pour Android n'accepte pas les extensions et les contournements (Edge Canary, forks Chromium tiers) sont expérimentaux. Le blocage fonctionne sur Chrome, Edge et Firefox de bureau.

---

## Navigateurs pris en charge

| Navigateur | Statut |
|---------|--------|
| Google Chrome | ✅ Entièrement pris en charge |
| Microsoft Edge | ✅ Entièrement pris en charge |
| Mozilla Firefox | ✅ Entièrement pris en charge |
| Autres navigateurs basés sur Chromium | ✅ Devrait fonctionner |

> **Note Firefox :** La version Firefox pour Android n’est pas encore activée (le manifeste ne déclare pas `gecko_android`) : AMO ne propose pour l’instant que la version bureau. Le reste des fonctions se comporte comme sous Chrome / Edge.

---

## Installation

| Store | Lien |
|---|---|
| Chrome Web Store | [Installer dans Chrome](https://chromewebstore.google.com/detail/iocnhglbdkdonajhkipknhgdnbombcic) |
| Microsoft Edge Add-ons | [Installer dans Edge](https://microsoftedge.microsoft.com/addons/detail/eigeengnoahojmfcnkkjnipbdnpngaod) |
| Modules complémentaires Firefox (AMO) | 🔜 En cours d’examen — le lien sera ajouté après publication |

> Installez uniquement depuis les boutiques officielles ci-dessus — évitez les sites de téléchargement tiers.

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

### Protection par mot de passe (optionnelle)

Vous ne faites pas confiance à votre propre bouton de contournement ? Définissez un mot de passe :

1. Ouvrez le popup → **⚙ / 🔒** → section *Protection par mot de passe*, ou le bouton 🔒 sur la page de liste
2. Définissez un mot de passe (min. 4 caractères) — il est stocké **uniquement sur cet appareil** sous forme de hachage salé, jamais envoyé
3. Ensuite, ces actions nécessitent le mot de passe :
   - Désactiver le blocage (interrupteur global)
   - Contournement 5 min sur la page de blocage
   - Supprimer un site ou vider la liste
   - Modifier une durée de blocage
4. Changez ou supprimez le mot de passe à tout moment (le mot de passe actuel est requis)

> ⚠️ **Un mot de passe oublié est irrécupérable.** Pas de lien de réinitialisation, pas de récupération, pas de porte dérobée — c'est voulu. Choisissez quelque chose dont vous vous souviendrez.

---

## Confidentialité

- **declarativeNetRequest** — Bloque les sites via des règles déclaratives. Ne lit pas le contenu des pages.
- **storage** — Sauvegarde votre liste de blocage en local. Aucune donnée envoyée.
- **Mot de passe (optionnel)** — Si défini, seul un hachage salé est stocké localement. Aucune synchronisation, aucun envoi. Un mot de passe oublié est irrécupérable.
- **alarms** — Gère les minuteurs de contournement temporaire. Aucun suivi en arrière-plan.
- **activeTab** — N'accède à l'onglet actif que lorsque vous interagissez avec l'extension.
- **Licence (optionnelle)** — Uniquement si vous activez une licence payante : la clé de licence et un identifiant d'installation aléatoire + des métadonnées du navigateur sont envoyées à `api.annmax1983.com` pour activer/valider la licence. Cela n'inclut jamais votre liste de blocage, votre historique de navigation ni vos données personnelles.
- Utilise la permission `<all_urls>` uniquement pour les règles de blocage `declarativeNetRequest`, et le serveur de licence uniquement pour l'activation payante. Aucun suivi. Aucun analytics. Les données des utilisateurs gratuits ne quittent jamais l'appareil.

**[📄 Politique de confidentialité complète](privacy-policy.html)**

---

## Avertissement relatif au droit d'auteur

Cette extension bloque uniquement les sites web spécifiés par l'utilisateur en local pour l'aider à maintenir sa concentration pendant le travail ou les études. L'extension ne modifie, ne copie ni ne redistribue aucun contenu de site web. Tous les droits de contenu des sites appartiennent à leurs éditeurs originaux.

## Licence

Copyright © 2026 JustFocus. Tous droits réservés.

---

> **Note :** le canal d'installation officiel est le Chrome Web Store, Microsoft Edge Add-ons et Firefox Add-ons (AMO). Ce dépôt contient la documentation et le code source de l'extension à titre de référence — ce n'est pas un canal de distribution, et aucun paquet hors ligne ou non signé n'y est publié.
