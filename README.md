# Carnet de biberons

Application web pour noter les biberons d'un bébé : date, heure et quantité enregistrées d'un appui, fiche du bébé (âge, poids, taille) et prévisions de lait selon l'âge.

Les données restent dans le navigateur de l'appareil (aucun serveur, aucun compte).

## Utiliser sur iPhone

1. Ouvrir l'adresse du site dans Safari.
2. Partager, puis « Sur l'écran d'accueil ».
3. Ouvrir le carnet depuis l'icône ajoutée et noter les biberons à partir de là.

## Fichiers

- `index.html` : toute l'application
- `manifest.webmanifest`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` : icône et réglages d'installation
- `sw.js` : ouverture hors connexion

## Réglages et nouveautés

- **Minuteur** : l'écran Biberons affiche « il y a … » depuis le dernier biberon, avec l'heure du prochain.
- **Donné par** : chaque téléphone peut renseigner son prénom (« Fiche et réglages »). Pour que les prénoms soient partagés entre les deux téléphones, copier `firestore.rules` dans Firebase (Firestore, onglet Règles, puis Publier). Sans cela, l'application fonctionne quand même, sans les prénoms.
- **Balayage** : glisser un biberon vers la gauche le supprime (bouton Annuler pendant quelques secondes).
- **Bilan** : navigation par semaine, statistiques, répartition par personne et heures des biberons.
- **Thèmes** : trois couleurs et mode clair, sombre ou automatique.
