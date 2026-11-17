# Graphix

Trace des fonctions et change leurs paramètres en direct : déplace-toi, zoome, lis les valeurs, et laisse l'appli trouver les zéros, les extremums et les intersections.

*English version: [README.en.md](README.en.md)*

![Graphix](screenshots/1.jpg)

## Version téléphone

- Le graphique est en haut, les fonctions et les curseurs en dessous.
- Glisse un doigt pour te déplacer, **pince à deux doigts** pour zoomer (ou les boutons − et +).
- Les fichiers exportés s'enregistrent dans le dossier Téléchargements/NeoDex du téléphone.
- Les mêmes fonctions que sur PC (même identifiant `neodex.graphix`).

## Écrire une fonction

Jusqu'à **6 fonctions** (f, g, h…), chacune avec sa couleur ; un clic sur le carré de couleur l'affiche ou la cache. L'écriture est naturelle :

- `2x`, `3sin(x)`, `(x+1)(x-1)` : la multiplication peut être sous-entendue ;
- `x^2`, `x²`, `x³`, `|x|`, `sin x`, `2,5` (virgule décimale) ;
- fonctions `sin cos tan asin acos atan sinh cosh tanh sqrt abs ln log exp floor ceil round sign min max mod`, constantes `pi` (ou `π`) et `e`.

Une faute est soulignée en rouge, et l'infobulle dit ce qui ne va pas. Les expressions sont lues par un petit analyseur maison : rien n'est exécuté comme du code.

## Paramètres

Les curseurs **a**, **b** et **c** (de -10 à 10, ou une valeur tapée) changent les courbes en direct. **t** est le temps : ▶ l'anime, pour voir `sin(x + t)` avancer.

## La vue

- **Glisser** pour se déplacer, **molette** pour zoomer autour de la souris, **⌂** pour revenir au centre.
- **Survoler** affiche x et la valeur de chaque fonction.
- **Dérivées en pointillés** ajoute la dérivée de chaque courbe.
- Les trous et les asymptotes (`1/x`, `tan x`) ne sont pas reliés.
- **Exporter en PNG** enregistre l'image du graphique.

## Points remarquables et table

- **Points remarquables** : les zéros, minimums, maximums et intersections dans la zone visible (marqués d'un carré blanc) ; un clic centre la vue dessus.
- **Table de valeurs** : x et chaque fonction, au pas de la grille.

## Données

Les fonctions, les curseurs et la vue sont gardés dans le dossier du plugin. Autorisation : `storage` seulement.

## Suites, nuages, aire et 3D

- **Suite** : écris avec `n` (`n^2/10`), ou `1 ; u*1,1` (u0 = 1, chaque terme = le précédent × 1,1). Les termes s'affichent en points et les premiers dans « Points remarquables ».
- **Nuage de points** : `(1;2) (2;3,5) (4;7)`. La droite de tendance (moindres carrés) est tracée en pointillés, avec son équation et r.
- **Aire sous la courbe** : le bouton colorie l'aire entre une courbe et l'axe des x et donne l'intégrale ; les bornes acceptent `pi/2`.
- **3D** : une expression avec `x` et `y` (`sin(x)*cos(y)`) passe la vue en 3D. Glisse pour tourner, molette pour zoomer.
