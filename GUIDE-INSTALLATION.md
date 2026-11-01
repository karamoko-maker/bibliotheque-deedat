# Bibliothèque Deedat v1.4 — Installer l'application sur le téléphone

L'application est une PWA : on la met en ligne gratuitement sur GitHub Pages, puis on l'installe depuis Chrome comme une vraie application (icône sur l'écran d'accueil, plein écran, fonctionne hors ligne pour les livres).

## Contenu du dossier

| Fichier | Rôle |
|---|---|
| `index.html` | L'application complète (livres, sourates, recherche, notes…) |
| `manifest.json` | Nom, couleurs et icônes de l'application |
| `sw.js` | Service worker : garde l'application disponible hors ligne |
| `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png` | Icônes |

Tous les fichiers sont à la racine : pas de sous-dossier, ce qui facilite l'envoi depuis un téléphone.

## 1. Mettre en ligne sur GitHub Pages

1. Sur github.com, créez un dépôt **public** nommé `bibliotheque-deedat`.
2. Dans le dépôt : **Add file → Upload files**, sélectionnez les 7 fichiers ci-dessus, puis **Commit changes**.
3. **Settings → Pages** : Source = *Deploy from a branch*, branche `main`, dossier `/ (root)`, puis **Save**.
4. Après 1 à 2 minutes, l'adresse s'affiche : `https://VOTRE-PSEUDO.github.io/bibliotheque-deedat/`

## 2. Installer sur Android

1. Ouvrez l'adresse dans **Chrome**.
2. Ouvrez **Réglages** dans l'application (menu ⋮ en haut à droite) et touchez **Installer**,
   ou bien : menu ⋮ de Chrome → **Installer l'application** (ou « Ajouter à l'écran d'accueil »).
3. L'icône « Deedat » apparaît sur l'écran d'accueil.

## 3. Installer sur iPhone

Safari → bouton **Partager** → **Sur l'écran d'accueil**.

## 4. (Optionnel) Créer un APK Android

1. Allez sur pwabuilder.com et collez l'adresse GitHub Pages.
2. **Package for stores → Android → Generate**, puis téléchargez le ZIP.
3. Installez l'APK sur le téléphone (autorisez « sources inconnues » si Android le demande).

## Audio du Coran

- **En ligne** : touchez une sourate puis **Écouter ici**. L'audio arrive en direct :
  arabe par Ali Al-Hudhaify (mp3quran.net), traduction française de Quran Central.
- Le mode **Arabe + fr.** enchaîne la récitation arabe puis la traduction, sourate après sourate.
- **Hors ligne** : téléchargez les MP3 voulus, puis ajoutez-les dans **Sourates → Mes fichiers audio**.
  Ils restent dans le téléphone et sont lus en priorité.

## Bibliothèque (livres PDF)

- Ouvrez **Bibliothèque**, touchez un lien de recherche pour trouver le PDF du livre et téléchargez-le.
- Revenez dans l'application et touchez **Ajouter mon PDF** : le livre reste dans le téléphone et s'ouvre dans la liseuse.
- La liseuse a besoin d'Internet la toute première fois, puis fonctionne hors ligne.

## Bon à savoir

- Favoris, notes et progression sont gardés dans le téléphone, propres à l'application installée.
  Ceux de la version ouverte dans Claude ne sont pas transférés.
- Pour mettre à jour : remplacez les fichiers sur GitHub par la nouvelle version.
  L'application se met à jour à la réouverture suivante (connexion internet nécessaire).
