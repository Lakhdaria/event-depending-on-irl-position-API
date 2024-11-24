# Geolocalisation Event 📍

Ce projet permet d'afficher dynamiquement du contenu spécifique en fonction de la localisation géographique de l'utilisateur. En utilisant les coordonnées GPS de l'utilisateur, le contenu correspondant à une zone spécifique est affiché lorsque l'utilisateur entre dans l'une des zones prédéfinies.

## Fonctionnalités ✨

- **Zones géographiques dynamiques** : Le projet contient plusieurs zones géographiques définies par des coordonnées et un rayon. Si l'utilisateur entre dans l'une de ces zones, un contenu spécifique à cette zone est affiché.
- **Contrôle de la position de l'utilisateur** : Utilisation de l'API de géolocalisation pour obtenir la position de l'utilisateur en temps réel.
- **Affichage conditionnel** : Le contenu est affiché uniquement si l'utilisateur se trouve dans une zone spécifique, définie par un rayon autour de coordonnées géographiques données.

## Technologies utilisées 💻

- **HTML** : Structure de la page et contenu dynamique.
- **JavaScript** : Calcul de la distance géographique et gestion de l'affichage en fonction de la position de l'utilisateur.
- **API de géolocalisation HTML5** : Utilisation de l'API de géolocalisation pour obtenir la position de l'utilisateur.

## Fonctionnement 🛠️

1. **Définition des zones** : Trois zones sont définies dans le script avec des coordonnées géographiques (latitude et longitude) et un rayon spécifié en mètres.
2. **Vérification de la position de l'utilisateur** : Lors de l'ouverture de la page, la position de l'utilisateur est récupérée via l'API de géolocalisation. Ensuite, une fonction de calcul de distance vérifie si l'utilisateur se trouve à l'intérieur de l'une des zones définies.
3. **Affichage dynamique du contenu** : En fonction de la zone dans laquelle l'utilisateur se trouve, un contenu spécifique est affiché. Si l'utilisateur quitte la zone, le contenu disparaît.

## Exemple de code 📜

Le code HTML est simple et contient trois sections `div` pour les trois zones, avec un style par défaut de `display: none`. Le JavaScript calcule la distance entre la position de l'utilisateur et les zones définies, puis affiche ou masque les éléments HTML en conséquence.

### Code HTML :

```html
<div id="elementZone1" style="display:none;">
    <h1>Bienvenue dans la zone 1! 🎉</h1>
    <p>Ce contenu est uniquement visible lorsque vous êtes dans la zone 1.</p>
</div>

<div id="elementZone2" style="display:none;">
    <h1>Bienvenue dans la zone 2! 🌍</h1>
    <p>Ce contenu est uniquement visible lorsque vous êtes dans la zone 2.</p>
</div>

<div id="elementZone3" style="display:none;">
    <h1>Bienvenue dans la zone 3! 🚀</h1>
    <p>Ce contenu est uniquement visible lorsque vous êtes dans la zone 3.</p>
</div>
