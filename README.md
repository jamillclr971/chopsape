# Chop'Sape

Application web qui propose chaque jour une tenue selon la météo et votre garde-robe.

- La météo du jour vient d'Open-Meteo (sans clé) pour une ville ou votre position, et reste réglable à la main.
- Le moteur compare l'isolation de la tenue (en clo) à celle qu'il faut pour la température ressentie, puis tient compte de la pluie, de l'occasion, des couleurs et de ce que vous avez porté ces derniers jours.
- Les vêtements et les photos restent dans le navigateur (IndexedDB), sur l'appareil. Rien n'est envoyé à un serveur, hors requêtes météo.
- L'onglet Garde-robe propose un export et un import JSON pour sauvegarder ou changer d'appareil.

## Publier sur GitHub Pages

1. Créez un dépôt GitHub (par exemple `chopsape`) et déposez-y les fichiers de ce dossier : `index.html`, `manifest.webmanifest`, `sw.js`, `icon.svg`, `.nojekyll`.
2. Dans le dépôt : Settings, Pages, Source « Deploy from a branch », branche `main`, dossier `/ (root)`.
3. Après une minute, le site est en ligne sur `https://<votre-compte>.github.io/chopsape/`.

Sur téléphone, ouvrez l'adresse puis « Ajouter à l'écran d'accueil » pour l'utiliser comme une application. La géolocalisation et le mode hors ligne demandent HTTPS, que GitHub Pages fournit.

## Limites

Les données sont liées au navigateur et à l'adresse du site. Vider les données du site les efface : exportez de temps en temps.
