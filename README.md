# Planétaire du système solaire

Modèle 3D interactif du Soleil, des planètes, de Cérès, de Pluton et de 22 satellites, positionnés selon les éphémérides réelles à la date choisie.

## Publier avec GitHub Pages

1. Créez un dépôt sur GitHub (par exemple `systeme-solaire`).
2. Déposez-y le contenu de ce dossier (`index.html`, le dossier `tex/` et ce fichier) à la racine du dépôt.
3. Dans le dépôt : **Settings → Pages → Build and deployment**, choisissez **Deploy from a branch**, branche `main`, dossier `/ (root)`, puis **Save**.
4. Après une minute environ, le site est en ligne à l'adresse `https://<votre-nom>.github.io/systeme-solaire/`.

## Tester en local

Ouvrir `index.html` directement fonctionne en partie, mais les textures de la Terre et de la Lune exigent un petit serveur :

```
python3 -m http.server 8000
```

puis ouvrir http://localhost:8000.

## Sources et crédits

- Positions des planètes : éléments képlériens du JPL (E. M. Standish), valables de 1800 à 2050.
- Orientation des astres : rapports du groupe de travail de l'UAI sur les éléments de rotation.
- Textures de la Terre et de la Lune : exemples du projet three.js (licence MIT), d'après des images de la NASA.
- Rendu 3D : three.js r128, chargé depuis cdnjs et jsDelivr.
