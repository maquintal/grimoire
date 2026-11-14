# Méthode d’adaptation des recettes

L’objectif n’est pas de faire entrer mécaniquement une recette dans BeerSmith avec une règle de trois. Il faut comprendre ce que la recette cherche à produire, ce qui ne convient pas au système actuel, puis proposer une adaptation justifiée avec ses compromis.

## Principe de base

Une recette peut ne pas « fitter » dans BeerSmith pour plusieurs raisons différentes : volume de brassin, profil d’équipement mal configuré, capacité de la cuve d’empâtage, quantité de grain, volume pré-ébullition, ingrédient indisponible ou paramètre de procédé. Il faut identifier le problème avant de modifier les quantités.

Les calculs restent nécessaires pour vérifier les volumes, les rendements, l’amertume, la densité ou la quantité de levure. Ils ne suffisent pas à décider si une substitution ou une mise à l’échelle préservera le caractère de la bière. Certains effets dépendent de la composition et du procédé; toutes les quantités ne se comportent pas comme de simples proportions.

L’efficacité de brassage de l’équipement n’est pas encore mesurée de façon fiable. Utiliser **72 % de brew efficiency** comme hypothèse provisoire quand la recette ne fournit pas de valeur. Si une capture ou les paramètres d’une recette indiquent une autre valeur, retenir cette valeur pour l’analyse de cette recette et signaler l’écart; ne pas la remplacer silencieusement par 72 % ni considérer une valeur isolée comme le rendement réel désormais établi. Voir [Équipement et planification des volumes](equipement-volumes.md) pour les données à consigner afin d’affiner cette estimation avec l’expérience.

## Démarche d’analyse

1. **Comprendre la bière recherchée.** Identifier le style, les caractéristiques importantes et les éléments qui définissent la recette : par exemple le caractère fumé, l’acidité, le corps, l’amertume ou le profil de fermentation.
2. **Localiser la contrainte.** Vérifier si le problème concerne BeerSmith, le volume visé, l’équipement, le procédé, un ingrédient indisponible ou plusieurs de ces éléments.
3. **Séparer l’essentiel du flexible.** Évaluer quels ingrédients et étapes sont déterminants pour le style et lesquels peuvent varier sans perdre l’intention de la recette.
4. **Analyser le rôle des ingrédients.** Une substitution doit être choisie pour sa fonction dans la recette et son effet attendu, pas seulement parce que son nom ou sa catégorie semble similaire. Expliquer les différences de goût, de fermentation et de comportement dans le procédé.
5. **Intégrer les contraintes réelles.** Utiliser les capacités mesurées du chaudron et de la cuve d’empâtage, les méthodes de rinçage disponibles, les pertes observées et les ingrédients réellement accessibles. Voir [Équipement et planification des volumes](equipement-volumes.md), [Levures](levures.md), [Houblons et substitutions](houblons.md) et [Malts et substitutions](malts.md).
6. **Comparer des options si nécessaire.** Quand plusieurs adaptations sont plausibles, comparer leur fonction, leur contribution sensorielle et leurs effets sur le procédé. Présenter les compromis plutôt que de prétendre qu’il existe un remplacement exact; ne pas faire d’une règle de trois ou d’une égalité de poids la justification principale.
7. **Vérifier dans BeerSmith.** Une fois les choix expliqués, recalculer la recette et contrôler les volumes à chaque étape, la densité, l’amertume, la couleur, le profil de fermentation et les limites des cuves. Relever l’efficacité de brassage de la recette; en son absence, utiliser l’hypothèse provisoire de 72 %.
8. **Signaler les incertitudes.** Distinguer les données connues des estimations. Si une donnée déterminante manque — par exemple le volume utile d’une cuve ou le format d’un ingrédient — ne pas inventer une valeur ni présenter le résultat comme définitif.

## Informations utiles pour une demande d’adaptation

Fournir autant que possible :

- la recette complète et sa source, y compris les quantités, étapes et paramètres BeerSmith;
- le volume de brassin attendu et le point de mesure visé (par exemple en fermenteur);
- les ingrédients de la recette qui sont indisponibles et l’inventaire pertinent;
- les contraintes d’équipement ou de procédé qui empêchent la recette de fonctionner;
- les caractéristiques du style ou du résultat que l’on veut absolument préserver;
- les compromis acceptables, comme une acidité ou une intensité fumée différente.

Les données déjà documentées dans ce dépôt — notamment l’[inventaire des levures](levures.md), les [houblons et substitutions](houblons.md), les [malts et substitutions](malts.md) et les [volumes de l’équipement](equipement-volumes.md) — doivent être réutilisées. Les ingrédients déjà apparus dans une recette ne prouvent pas à eux seuls qu’ils sont en stock. Il ne faut pas demander à l’utilisateur de répéter les données connues, sauf si elles doivent être confirmées ou mises à jour.

## Format de réponse attendu

Pour chaque adaptation proposée :

- résumer le problème repéré et son origine probable;
- expliquer le rôle des ingrédients ou étapes qui changent;
- proposer une adaptation principale et, si utile, une autre option;
- décrire les différences attendues par rapport à la recette d’origine;
- montrer les contrôles BeerSmith et les calculs qui vérifient la proposition;
- nommer les données manquantes, les hypothèses et le degré de confiance.

Ne pas qualifier une bière d’identique à l’originale si des ingrédients ou des procédés déterminants ont changé. L’objectif est une adaptation cohérente et réalisable, dont les compromis sont compris.
