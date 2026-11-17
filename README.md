# Services.FUN — V5 : Présentations + Grand Quiz

Prototype pédagogique local pour l'animation des services de **Leroy Merlin Calais**. Maquette interne non officielle, indépendante des systèmes du magasin.

## Nouveau fonctionnement

**1. Présentations par service**

La page d'accueil comporte six mascottes et six univers : Livraison, Financement, Service pose, Location, Service après-vente (SAV), Retrait 2 h.

En ouvrant un service, on trouve **ses propres diaporamas**. L'organisateur peut créer, renommer, dupliquer et supprimer des présentations ; ajouter, modifier, dupliquer, supprimer et réordonner leurs diapositives ; choisir une mise en page et une transition ; lancer une lecture plein écran.

Les **8 dispositions** proposées sont : Couverture, Points clés, Texte + image, Photo plein cadre, Vidéo, Étapes du parcours, Message à retenir, Conclusion. Chaque diapo possède plusieurs palettes, des notes d'animation et des transitions : fondu, glissement, zoom, bascule ou aucune. Images par URL HTTPS ou import PNG/JPG/WEBP réduit automatiquement. Vidéos intégrées via URL YouTube ou lien MP4 HTTPS ; pas d'hébergement vidéo local dans ce prototype.

**Pour présenter :** cliquer sur « Lire » puis sur la diapositive / « Suivante », ou utiliser les flèches gauche et droite. **Échap** ferme le diaporama. Le bouton **Plein écran** sollicite le plein écran du navigateur quand autorisé.

**2. Grand Quiz des Services**

Les quiz ne sont **plus dans chaque service**. Le menu « Grand Quiz des Services » regroupe les **12 formats de jeux** : QCM A/B/C/D, question avec image, vrai/faux, sondage, cartes à associer, mots croisés, mots mêlés, étapes à remettre dans l'ordre, devinette, mot manquant, diapo explicative et diapo vidéo. L'organisateur peut construire une partie mêlant les six services et choisir le service concerné par chaque question.

L'éditeur QCM conserve **la question en largeur totale**, **A/B sur la ligne supérieure**, **C/D sur la ligne inférieure** et un grand bloc **Bonne réponse**. Les jeux et anciens parcours de démonstration de la V4 sont conservés et accessibles depuis cet espace. Un **Grand Quiz des Services** mélangé est créé comme exemple lors de la première utilisation de la V5.

## Installation et essai

- **Essai immédiat :** télécharger `Services_FUN_Demo_V5.html`, puis l'ouvrir dans un navigateur. Le fichier contient CSS, JavaScript et six illustrations embarquées : pas de serveur nécessaire pour l'interface (les liens vidéo distants nécessitent Internet).
- **GitHub Pages :** publier `index.html`, `style.css`, `app.js`, `presentations.js` et le dossier `assets/` à la racine d'un dépôt dédié. Dans GitHub, Settings → Pages → Deploy from a branch → `main` / root. Ne pas confondre publication du code avec mise en ligne : cette archive n'est **pas** déjà publiée.

## Sauvegarde

Les présentations, quiz et résultats sont sauvegardés dans **localStorage sur le navigateur local**. Le bouton « Exporter les données » crée une sauvegarde JSON, réimportable depuis l'atelier du quiz. **Sauvegarder régulièrement en JSON**, notamment si vous ajoutez des images : le stockage du navigateur a une limite. Les anciennes données V4 stockées sous la même clé sont conservées à l'ouverture de la V5.

## Limites de cette maquette

Aucun compte sécurisé, aucune synchronisation en direct entre plusieurs téléphones, aucun hébergement des vidéos ou de base de données centralisée. Les présentations ne génèrent pas de fichier `.pptx` modifiable dans Microsoft PowerPoint ; il s'agit d'un **éditeur et lecteur de diaporama dans le navigateur**. Les quiz possèdent toujours un classement local et des livrets imprimables en PDF via le navigateur.

Les questions et supports sont des exemples à faire **valider par les référents du magasin**. Ne saisissez pas de données personnelles de clients, informations financières sensibles ou contenus internes confidentiels dans une page GitHub Pages publique. Les logos/marquages Leroy Merlin figurant dans les mascottes sont des illustrations générées pour la maquette, pas les fichiers officiels de charte graphique.
