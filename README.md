# AMANA PACKAGING

Application de stock, ventes et factures.

## Fichiers à mettre à la racine du dépôt GitHub
`index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png`, `package.json`, `capacitor.config.json`
et le fichier `.github/workflows/build-apk.yml` (dossier à créer).

## Fabriquer l'APK
1. Dépôt > Settings > Actions > General > Workflow permissions : choisir « Read and write permissions », puis Save.
2. Onglet Actions > « Build APK » > Run workflow (il se lance aussi à chaque envoi sur `main`).
3. Au bout de 5 à 10 minutes, ouvrez l'onglet Releases du dépôt : `AMANA-PACKAGING.apk` est dans la dernière version.
4. Téléchargez l'APK sur le téléphone et installez-le (autoriser l'installation depuis cette source).

## Site web (facultatif)
Settings > Pages > « Deploy from a branch » > `main` / `/ (root)`.

## Données
Elles sont enregistrées sur l'appareil. Dans l'APK, « Imprimer » et « Télécharger » ouvrent le partage Android : choisissez une application pour imprimer ou envoyer la facture.
