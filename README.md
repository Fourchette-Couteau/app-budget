# 💰 Mon Budget — Application PWA iOS

> Application de gestion budgétaire personnelle, conçue comme une PWA (Progressive Web App) optimisée pour iOS/Safari. Interface inspirée du design Liquid Glass d'Apple, entièrement en HTML/CSS/JS vanilla.

---

## 📱 Aperçu

Mon Budget est une application complète de gestion des finances personnelles. Elle fonctionne directement dans Safari sur iPhone, peut être ajoutée à l'écran d'accueil comme une vraie app native, et stocke toutes les données localement sur l'appareil (aucun serveur, aucun compte requis).

**Stack technique :** HTML · CSS · JavaScript vanilla · Chart.js · localStorage  
**Compatibilité :** Safari iOS 15+ · Chrome · Firefox  
**Stockage :** 100% local (localStorage), aucune donnée envoyée

---

## ✨ Fonctionnalités

### 🏠 Tableau de bord
- Solde de la période en cours (revenus − dépenses)
- **Projection fin de période** : solde estimé après toutes les récurrences à venir, calé sur ton jour de paie
- Taux d'épargne de la période
- Mini-widgets Score, Streak et Badges
- Graphique de répartition des dépenses (donut Chart.js)
- Barres de dépenses par catégorie
- Transactions récentes
- Prévision sur 6 mois (projection basée sur la moyenne des 3 derniers mois)
- Défi mensuel avec progression en temps réel

### ➕ Ajouter une transaction
- Formulaire Dépense / Revenu
- Saisie du montant, description, catégorie, date
- Catégories personnalisables (voir ci-dessous)

### 📋 Historique
- Liste complète de toutes les transactions
- **Recherche full-text** en temps réel
- **Filtres chips** : Tout, Dépenses, Revenus, + top catégories
- Total affiché (dépenses · revenus) selon le filtre actif
- Swipe gauche pour supprimer ou dupliquer une transaction
- Tap sur une transaction pour la modifier

### 💰 Épargne
Deux onglets :

**💰 Épargne classique**
- Versements et retraits avec historique
- Objectif d'épargne avec barre de progression
- Chaque versement est automatiquement déduit du solde de la période en cours
- Chip résumé des placements cliquable

**📈 Placements**
- Livret A (3%), LDDS (3%), PEL (2.25%), CEL (2%), Livret Jeune (4%), Assurance-vie (3.5%), Compte sur livret, Épargne salariale, Personnalisé
- Affichage du solde, taux, intérêts estimés annuels et mensuels
- Barre de remplissage du plafond réglementaire
- Mise à jour du solde directement depuis la carte
- **Récurrences sur placements** : virement automatique mensuel configurable (🔁)

### ⏰ Budgets
- Limite mensuelle par catégorie
- Indicateur €/jour restant
- Barre de progression visuelle
- Alerte si dépassement prévu

### 🔁 Récurrences
- Transactions récurrentes mensuelles (abonnements, loyer, salaire...)
- Choix du jour du mois
- Toggle actif/inactif
- **Total mensuel affiché** en haut de la section (dépenses + revenus récurrents)
- Modification et suppression

### 🧳 Partage de dépenses *(Réglages → Outils)*
- Créer un événement (trip, soirée, voyage...)
- Ajouter des participants
- Enregistrer les dépenses : qui a payé, divisé entre qui
- **Calcul automatique** : qui doit quoi à qui, avec solde net simplifié
- Plusieurs payeurs possibles par événement

### 🔔 Notifications
- Cloche en haut avec badge rouge (non lues)
- 5 types : budget dépassé, budget à 80%, fin de période, récurrences dues, récap quotidien
- Panel latéral droit avec blur
- Notifications non lues : plein · Notifications lues : assombries, trait coloré conservé
- Toggles on/off dans les Réglages

### 🏆 Gamification *(Réglages → Outils → Succès & Badges)*
- **Score /100** avec rang : S / A / B / C / D
- **Streak** : jours consécutifs d'utilisation
- **25 badges** répartis en 7 catégories (début, volume, épargne, budget, streak, score, défis)
- Historique du score sur 30 jours (sparkline)
- Toast à chaque nouveau badge débloqué

### 🎯 Défi mensuel
- 5 défis disponibles : Chef à domicile, Épargnant 10%, Budget parfait, Assidu (7j), Zen
- Sélecteur de défi via bouton ⟳
- Barre de progression en temps réel

### ✏️ Catégories personnalisées *(Réglages → Outils → Catégories)*
- **Catégories de base** : masquables/affichables individuellement
- **Catégories custom** : création avec emoji natif iOS + nom libre
- S'appliquent partout : Ajouter, Récurrences, Modification, Budgets, Historique

### 📊 Statistiques *(Réglages → Outils → Statistiques)*
- Stats annuelles avec sélecteur d'année
- Top catégories de dépenses
- Évolution mois par mois
- Section placements : total placé, intérêts estimés, répartition

### 🗓 Calendrier *(Réglages → Outils)*
- Vue mensuelle des transactions par jour

---

## 🎨 Design & Personnalisation

### Thèmes de couleur
6 thèmes disponibles dans Réglages → Apparence :
| Thème | Description |
|---|---|
| 🔵 Défaut | Bleu accent, orbes violets |
| 🌊 Océan | Bleu azur vers marine |
| 🌲 Forêt | Vert très sombre vers menthe |
| 🌅 Coucher | Rouge vif vers orange chaud |
| 🌙 Minuit | Violet profond vers lavande |
| 🌸 Rosé | Bordeaux vers rose vif |

Chaque thème colore : les orbes d'arrière-plan, la carte de solde, la barre de navigation.

### Mode clair / sombre
Automatique (suit les préférences système iOS) ou forcé manuellement.

### Tableau de bord personnalisable
8 éléments activables/désactivables : Score/Badges, Donut, Barres, Transactions récentes, Défi, Prévision, Impôts.  
Ordre de navigation réorganisable par drag & drop.

### Catégories favorites
Épingle tes catégories préférées pour les voir en premier dans les selects.

---

## ⚙️ Réglages

| Section | Contenu |
|---|---|
| Apparence | Thème dark/light, couleur |
| Transactions récurrentes | Gestion des récurrences |
| Alertes & Notifications | Toggles par type |
| Tableau de bord | Éléments affichés |
| Comptes | Multi-comptes (courant, joint, pro) |
| Général | Profil, PIN, devise, jour de paie |
| Outils | Calendrier, Stats, Badges, Perso, Catégories, Partage |
| Profil fiscal | Taux d'imposition |
| Partager | Rapport du mois, partager l'appli |
| Données | Export JSON/CSV, import, sauvegarde |
| Zone danger | Réinitialisation |

---

## 🏦 Multi-comptes *(Réglages → Comptes)*
- Activable via toggle
- Types : Compte courant, Compte joint, Compte pro, Personnalisé
- Barre de chips en haut de l'accueil pour switcher
- Solde total tous comptes affiché
- Chaque transaction est associée au compte actif

---

## 🔒 Sécurité & Données

- **Code PIN** style iOS (activable dans Réglages → Général)
- **Export JSON** : sauvegarde complète des données
- **Export CSV** : compatible Excel/Sheets
- **Import JSON** : restauration depuis une sauvegarde
- Aucune donnée transmise à un serveur — tout reste sur l'appareil

---

## 🚀 Installation sur iPhone

1. Ouvrir `budget.html` dans **Safari** sur iPhone
2. Appuyer sur le bouton **Partager** ↑
3. Sélectionner **"Sur l'écran d'accueil"**
4. Nommer l'app et confirmer

L'app s'installe comme une application native avec icône, écran de lancement et barre de statut immersive.

---

## 📁 Structure du projet

```
budget.html          ← Fichier unique (HTML + CSS + JS)
README.md            ← Ce fichier
```

Tout le projet tient dans un seul fichier HTML autonome, sans dépendance externe hormis Chart.js (chargé via CDN).

---

## 🛠 Développement

Ce projet a été entièrement développé en collaboration avec **Claude (Anthropic)**, en itérations successives sur plusieurs sessions. L'approche adoptée : une fonctionnalité à la fois, tests sur iPhone après chaque changement.

**Contraintes techniques respectées :**
- Zéro template literals (compatibilité Safari)
- Zéro spread operator dans les arrow functions
- `var` partout (éviter les conflits de redéclaration)
- Toutes les fonctions `render` utilisent la concaténation de chaînes

---

## 📝 Changelog résumé

| Version | Nouveautés |
|---|---|
| v1.0 | Core : transactions, historique, budgets |
| v2.0 | Récurrences, notifications |
| v3.0 | Épargne + objectifs |
| v4.0 | Gamification (badges, score, streak) |
| v5.0 | Personnalisation, thèmes, catégories fav |
| v6.0 | Placements multiples, multi-comptes |
| v6.5 | Prévision 6 mois, défi perso, historique scores |
| v6.8 | Épargne déduite du solde, projection récurrences |
| v6.9 | Catégories personnalisées complètes |
| v7.0 | Partage de dépenses (trips, soirées) |

---

*Projet personnel — non publié sur l'App Store — usage privé*
