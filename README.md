# SOLUL 🇸🇳

**Marketplace de mode sénégalaise** — Achetez, vendez et louez des vêtements traditionnels et modernes entre particuliers.

SOLUL est une application mobile React Native qui permet de revendre ou louer des tenues africaines (boubous, robes, tuniques, accessoires…) de seconde main, avec une expérience 100 % locale pensée pour le Sénégal.

---

## 📱 Fonctionnalités

- **Authentification** — Inscription, connexion, vérification par code, mot de passe oublié
- **Boutique** — Catalogue avec filtres par genre (Femmes, Hommes, Enfants), prix, recherche
- **Détail article** — Photos, description, état, matière, localisation vendeur
- **Proposition de prix** — Marchandage intégré avec bouton OK de validation
- **Panier & Paiement** — Wave, Orange Money, Free Money (simulé)
- **Confirmation d'acquisition** — Suivi des commandes avec bouton "J'ai reçu ma commande"
- **Mise en vente / location** — Formulaire complet avec sélection photos (galerie + caméra)
- **Messagerie** — Chat en temps réel entre acheteur et vendeur
- **Avis & Notes** — Système d'évaluation des vendeurs avec réponses aux commentaires
- **Favoris** — Sauvegarde d'articles pour plus tard
- **Notifications** — Propositions de prix, paiements, commandes
- **Profil** — Gestion du compte, articles publiés

> ⚠️ L'application fonctionne entièrement en **localStorage** (AsyncStorage) avec des données fictives. Aucun backend n'est nécessaire.

---

## 🛠️ Stack technique

| Technologie | Version |
|---|---|
| React Native | 0.81.5 |
| Expo SDK | 54 |
| TypeScript | 5.9 |
| React Navigation | 7.x |
| AsyncStorage | 2.1 |
| expo-image-picker | 17.0 |

---

## 🚀 Lancer le projet

### Prérequis

- [Node.js](https://nodejs.org/) (v18 ou supérieur)
- [Expo Go](https://expo.dev/go) installé sur votre téléphone (iOS ou Android)
- Un ordinateur et un téléphone **connectés au même réseau Wi-Fi**

### Installation

```bash
# 1. Cloner le dépôt
git clone https://github.com/thesombrecoder18/solul.git
cd solul

# 2. Installer les dépendances
npm install

# 3. Lancer le serveur de développement
npx expo start
```

### Ouvrir sur mobile avec Expo Go

1. Après `npx expo start`, un **QR code** s'affiche dans le terminal
2. **Android** : Ouvrez l'app Expo Go → scannez le QR code
3. **iPhone** : Ouvrez l'app Appareil photo → scannez le QR code → ça ouvre Expo Go automatiquement

> 💡 Si le QR code ne fonctionne pas, appuyez sur `s` dans le terminal pour passer en mode **Expo Go**, puis rescannez.

### Comptes de test

L'application est pré-remplie avec des utilisateurs fictifs. Vous pouvez vous connecter avec :

| Email | Mot de passe |
|---|---|
| binta@gmail.com | binta123 |
| khoudia@gmail.com | khoudia123 |
| modou@gmail.com | modou123 |
| bilalman08@gmail.com | bilal123 |

Ou créez votre propre compte via l'écran d'inscription.

---

## 📂 Structure du projet

```
solul/
├── App.tsx                    # Point d'entrée + Navigation
├── src/
│   ├── components/ui/         # Composants réutilisables (ProductCard, InputField…)
│   ├── constants/             # Couleurs, espacements, tailles de police
│   ├── data/                  # Données fictives (produits, utilisateurs, conversations)
│   ├── screens/               # 20 écrans de l'application
│   │   ├── SplashScreen       # Écran de démarrage
│   │   ├── LoginScreen        # Connexion
│   │   ├── RegisterScreen     # Inscription
│   │   ├── HomeScreen         # Accueil / Boutique
│   │   ├── ProductDetailScreen # Détail d'un article
│   │   ├── CartScreen         # Panier
│   │   ├── PaymentScreen      # Paiement
│   │   ├── SellScreen         # Mise en vente / location
│   │   ├── ChatScreen         # Messagerie
│   │   ├── ReviewsScreen      # Avis vendeur
│   │   ├── ProfileScreen      # Profil utilisateur
│   │   └── ...                # Et plus encore
│   ├── services/              # Services (auth, cart, product, message, storage)
│   └── types/                 # Types TypeScript
├── package.json
└── tsconfig.json
```

---

## 🎨 Design

- **Couleur primaire** : `#8B6914` (or)
- **Fond** : `#F5E6D0` (beige)
- **Texte** : `#3D2B1F` (brun foncé)

L'interface s'inspire des couleurs chaudes et terreuses de la mode sénégalaise.

---

## 📝 Notes

- Les données sont stockées localement via AsyncStorage. **Désinstaller l'app efface toutes les données.**
- Les images produits et profils sont chargées depuis Unsplash (connexion internet requise).
- L'app se ré-initialise automatiquement avec les données fictives si le stockage est vide.

---

## 👥 Auteurs

Projet réalisé dans le cadre d'un cours d'entrepreneuriat.

---

## 📄 Licence

Ce projet est à usage éducatif.
