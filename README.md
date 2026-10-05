# Rayon

Back office mobile pour l'achat-revente sur Vinted : lots, stock, ventes, bénéfice, temps passé et générateur d'annonces.

## Mettre en ligne sur GitHub Pages

1. Crée un dépôt sur GitHub, par exemple `rayon` (il peut être privé si tu as GitHub Pro, sinon public).
2. Dépose les 7 fichiers de ce dossier à la racine du dépôt :
   `index.html`, `manifest.webmanifest`, `sw.js`, `icon-180.png`, `icon-192.png`, `icon-512.png`, `README.md`.
   (Depuis le site : « Add file » → « Upload files ».)
3. Dans le dépôt : **Settings → Pages → Source : Deploy from a branch → Branch : `main` / `(root)` → Save**.
4. Une minute plus tard, l'app est en ligne sur `https://<ton-pseudo>.github.io/rayon/`.

## L'installer sur ton téléphone

- **iPhone (Safari)** : ouvre l'adresse → bouton Partager → « Sur l'écran d'accueil ».
- **Android (Chrome)** : menu ⋮ → « Installer l'application ».

Utilise toujours l'app depuis l'icône de l'écran d'accueil : sur iPhone, l'app installée et Safari ont chacune leur propre mémoire, et Safari peut effacer les données d'un site non installé après quelques semaines sans visite.

## Où sont tes données

Tout est enregistré **dans le navigateur de ton téléphone** (localStorage pour les données, IndexedDB pour les photos). Rien n'est envoyé sur internet, et rien n'est stocké sur GitHub.

Conséquence : si tu changes de téléphone ou vides les données du navigateur, elles disparaissent. Fais une sauvegarde régulière : **Plus → Sauvegarde → Télécharger la sauvegarde** (ou « Copier » et colle-la dans une note). Pour restaurer : **Importer un fichier .json**. Les photos ne sont pas incluses dans la sauvegarde.

## Mettre à jour l'app

Remplace `index.html` dans le dépôt, puis change `VERSION` en haut de `sw.js` (ex. `rayon-v2`) pour forcer le téléphone à charger la nouvelle version. Tes données ne sont pas touchées par une mise à jour.
