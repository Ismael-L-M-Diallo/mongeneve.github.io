# MonGeneve

MonGeneve est une application web cartographique interactive qui affiche des lieux de Genève avec des points colorés, des notes sur 10, des informations de prix, des liens web et une géolocalisation GPS.

## Fonctionnalités

- Carte interactive basée sur Leaflet.
- Marqueurs colorés selon le type de lieu.
- Bandeau avec le blason de Genève.
- Filtres par catégorie.
- Liste des lieux visibles.
- Top 3 des meilleurs lieux par catégorie.
- Bouton de recentrage sur Genève.
- Géolocalisation GPS de l’utilisateur.
- Liens web et prix visibles dans les infobulles.

## Fichiers

- `geneve-explorer-no-default-selection.html` : application principale.
- `image.jpg` : image du blason utilisée dans le bandeau.

## Utilisation

1. Ouvrir le fichier HTML dans un navigateur moderne.
2. Activer les catégories souhaitées via les filtres.
3. Utiliser les boutons pour recharger, recentrer ou se localiser.

## Structure

- `aside` : panneau latéral avec image, filtres, résumé et listes.
- `main` : carte Leaflet.
- JavaScript embarqué : chargement des lieux, filtres, marqueurs, popups et GPS.

## Données

Les lieux affichés sont intégrés dans le fichier HTML sous forme de tableau JavaScript. Chaque entrée contient :

- le type de lieu,
- le nom,
- la latitude,
- la longitude,
- la note sur 10,
- des métadonnées optionnelles comme le site web.

## Personnalisation

Pour modifier l’application :

- ajouter ou retirer des lieux dans le tableau `A`,
- changer les couleurs dans les variables CSS `:root`,
- remplacer l’image du bandeau par un autre fichier local,
- ajuster les notes, catégories ou labels.

## Dépendances

- Leaflet via CDN.
- Google Fonts via CDN.
- Connexion Internet requise pour les tuiles de carte et les ressources externes.

## Remarques

- L’application fonctionne sans serveur local si le navigateur autorise l’ouverture du fichier HTML.
- La géolocalisation GPS peut demander une autorisation utilisateur.
