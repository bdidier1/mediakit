# Clip2EP – Media kit

Site officiel de **Clip2EP**, créateur de contenu sur les parcs d'attractions (TikTok et YouTube). Il sert de **media kit** pour les marques et les parcs : présentation, audience, partenariats, vidéos et contact.

## Points forts

- **Accueil en 3D** : un parc d'attractions interactif (Three.js) où chaque attraction mène à une section du site ; plan 2D de secours si la 3D n'est pas disponible
- **Statistiques d'audience à jour** : abonnés, j'aime et vues des vidéos, récupérés **chaque nuit** par une GitHub Action (yt-dlp + API YouTube) puis enregistrés dans `stats/stats_compact.json`
- **Page « Mes vidéos »** : toutes les vidéos TikTok et YouTube, avec leurs vignettes conservées dans le site (les adresses d'origine expirent)
- **Partenariats** : parcs et marques avec lesquels j'ai travaillé
- **Site multilingue** et thème clair / sombre

## Technologies

HTML, CSS, JavaScript (modules), Three.js, Python (script de mise à jour), GitHub Actions.

## Lancer en local

```bash
python -m http.server 8000
```

puis ouvrir http://localhost:8000.

La clé de l'API YouTube utilisée par la GitHub Action est un **secret du dépôt** (`YOUTUBE_API_KEY`), jamais écrite dans le code.
