# LudoPilot Voyages · V1

Application web iPhone pour Ludo aux Philippines et Lisa en Thaïlande, utilisable dans tous les pays. L’interface est en français et l'écran chauffeur permet de choisir français, anglais, thaï, tagalog, indonésien et espagnol.

## Installation depuis l’iPhone sans Mac

1. Sur GitHub, dans le dépôt public `ludopilot-voyages`, ouvrir **Add file > Upload files**.
2. Sélectionner les cinq fichiers `index.html`, `sw.js`, `manifest.webmanifest`, `icon.svg`, `icon-180.png` dans le dossier téléchargé **LudoPilot-Voyages**. Les placer à la racine du dépôt, pas dans un sous-dossier. Cliquer sur **Commit changes**.
3. Dans **Settings > Pages**, sélectionner **Deploy from a branch**, branche **main**, dossier **/(root)**, puis enregistrer.
4. Le site devrait être disponible à `https://ubud64.github.io/ludopilot-voyages/` après publication. Ouvrir le lien depuis Safari puis **Partager > Sur l'écran d'accueil**. Lisa peut utiliser le même lien.

## Fonctionnement

- Voyage : saisir départ, arrivée et éventuellement passage obligé, sélectionner avec ou sans avion.
- Étapes : préparer et suivre chaque segment indépendamment, y compris les correspondances.
- Chauffeur : destination du segment actif uniquement, en gros caractères; langue du chauffeur personnalisable. Les suggestions « Automatique » ne sont que des heuristiques : vérifier le pays et choisir la bonne langue au besoin.
- Réglages : raccordement facultatif au moteur existant Cloudflare Worker via son URL de base **HTTPS**, sauvegarde/export des voyages JSON.

Sans connexion du moteur, la recherche automatique ne fonctionne pas encore; création manuelle disponible dès l'installation. Ne jamais saisir ni publier les clés API OpenAI ou Google. Le moteur externe peut entraîner des frais API.

Les voyages sont stockés localement sur chaque téléphone et ne sont pas visibles par l'autre personne. Pour préserver les voyages, utiliser **Réglages > Exporter JSON**. Le site et les voyages sauvegardés peuvent rester accessibles sans connexion après une première ouverture en ligne. Les cartes Google, les horaires, les recherches et les services externes requièrent en revanche Internet. Les traductions du bouton chauffeur sont indicatives, notamment dans les langues asiatiques.
