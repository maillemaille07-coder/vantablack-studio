# Vantablack Studio : site

Site statique (aucune installation, aucun build). Pages : `index.html`, `projets.html`, `tarifs.html`, `contact.html`.
Les polices, logos et vidéos sont dans `assets/`. `support.js` fait tourner les pages : ne pas le modifier ni le supprimer.

## Mettre en ligne avec GitHub Pages
1. Créer un compte sur github.com, puis un dépôt **public** nommé par exemple `vantablack-studio`.
2. Sur la page du dépôt : **Add file → Upload files**, puis glisser tout le contenu de ce dossier (fichiers et dossier `assets`). Limites de GitHub : 100 fichiers par envoi (ici 41) et 25 Mo par fichier (le plus lourd fait 13 Mo). Valider avec **Commit changes**. Les fichiers cachés `.nojekyll` et `README.md` sont facultatifs.
3. Sur GitHub : **Settings → Pages → Build and deployment → Source : Deploy from a branch**, branche `main`, dossier `/ (root)`.
4. Le site apparaît à `https://<ton-compte>.github.io/vantablack-studio/` après 1 à 2 minutes.
5. Domaine perso : dans **Settings → Pages → Custom domain**, saisir `vantablack-studio.fr` (ou `www.`), puis chez le registrar ajouter les enregistrements DNS indiqués par GitHub (4 enregistrements A vers 185.199.108.153, .109.153, .110.153, .111.153, et un CNAME pour `www`). Cocher ensuite **Enforce HTTPS**.

## Modifier le site plus tard
Remplacer un fichier dans le dépôt (par exemple `projets.html`), puis valider (commit) : GitHub Pages republie tout seul.
