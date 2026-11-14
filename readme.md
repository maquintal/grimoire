# Brassage maison

Ce dépôt a pour objectif de m’aider à optimiser la fabrication de bière maison, notamment lorsque des recettes trouvées ailleurs ne correspondent pas à mon équipement ou aux ingrédients disponibles. Le brassage dépend de nombreux paramètres — style recherché, ingrédients, équipement, procédé et fermentation — qu’il faut analyser ensemble.

Les fichiers Markdown de ce dépôt constituent un contexte de référence pour échanger avec des agents d’intelligence artificielle. Les calculs sont utiles pour vérifier une adaptation, mais ne remplacent pas l’analyse du rôle des ingrédients, du style visé, des contraintes du système et des compromis sur le résultat.

## Références

- [Skill d’adaptation des recettes](.github/skills/adapter-recettes/SKILL.md) — consignes réutilisables pour analyser et adapter les recettes avec le contexte du dépôt.
- [Méthode d’adaptation des recettes](adapter-recettes.md) — analyser le style, les ingrédients, BeerSmith et les contraintes de l’équipement avant de proposer des changements.
- [Fermentation](fermentation.md) — procédé actuel en une étape, distinction avec une fermentation en deux étapes et critères avant embouteillage.
- [Interpréter les alertes Run Checks de BeerSmith](beersmith-run-checks.md) — interprétation des avertissements de levure, de pH d’empâtage et de couleur.
- [Houblons et substitutions](houblons.md) — choisir un remplacement selon la fonction du houblon et ajuster l’amertume dans BeerSmith.
- [Malts et substitutions](malts.md) — comparer les malts selon leur fonction, leur contribution sensorielle et leur comportement à l’empâtage.
- [Choisir un guide de style](styles-biere.md) — choisir BJCP ou Brewers Association dans BeerSmith et interpréter les plages sans les traiter comme des règles absolues.
- [Adaptation de la Roggenbier](roggenbier/optimisation-roggenbier.md) — remplacements du Magnum et de la M20, et contraintes de la recette face à l’équipement réel.
- [Levures](levures.md) — inventaire des levures disponibles pour adapter les recettes aux produits que je peux acheter.
- [Remplacer WLP677 dans une Lichtenhainer](lichtenhainer/remplacer-wlp677-lichtenhainer.md) — comparaison avec WildBrew Philly Sour, l’option acidifiante de la liste.
- [Optimisation de la Lichtenhainer dans BeerSmith](lichtenhainer/optimisation-lichtenhainer.md) — lecture des écarts de style, pistes d’adaptation et points à confirmer.
- [Interpréter l’onglet Yeast de BeerSmith](beersmith-yeast.md) — taux d’ensemencement, cellules nécessaires, nombre de sachets et conséquences d’un surdosage.
- [Équipement et planification des volumes](equipement-volumes.md) — cuve d’empâtage, chaudron, ratio eau/grain, batch sparging et volume en fermenteur.