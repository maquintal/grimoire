# Fermentation

Ce document consigne le procédé actuel de fermentation et sa traduction dans BeerSmith. Il distingue le nombre de phases du procédé, le nombre de levures utilisées et le temps passé dans le fermenteur.

## Procédé actuel

Le procédé décrit par l’utilisateur est :

1. transférer le moût dans un fermenteur;
2. ajouter la ou les levures retenues pour la recette;
3. laisser fermenter environ 30 jours;
4. embouteiller lorsque la fermentation est terminée.

La bière reste dans un seul fermenteur jusqu’à l’embouteillage. Pour un procédé sans seconde phase distincte de température ou de fermentation, le profil **Ale, Single Stage** dans BeerSmith correspond à cette méthode. La capture actuelle de la Lichtenhainer utilise ce profil.

## Ce que signifie « une étape »

- **Single Stage** décrit un profil de fermentation à une étape; ce n’est ni le nombre de souches ajoutées ni la durée totale passée dans le fermenteur.
- Une attente de 30 jours dans le même fermenteur ne crée pas à elle seule une deuxième étape.
- Une période de maturation dans le même fermenteur peut faire partie du temps total sans constituer une seconde phase de fermentation.
- Une phase distincte, par exemple un changement de température planifié après la fermentation principale, peut demander un profil à plusieurs étapes même sans transfert vers un autre fermenteur.
- Le réglage **Two Stage Yeast Starter** de l’onglet **Yeast** concerne un starter en deux étapes; il ne correspond pas au profil de fermentation « Two Stage ».
- Le nombre de levures ou de cultures ajoutées est un choix indépendant du profil de fermentation. Pour un remplacement avec Philly Sour, voir [l’analyse de la Lichtenhainer](lichtenhainer/optimisation-lichtenhainer.md).

## Durée et embouteillage

Les 30 jours sont le délai prévu par le procédé actuel, pas une garantie que toute fermentation sera terminée à cette date. Avant l’embouteillage, vérifier que la densité est stable sur plusieurs mesures prises à plusieurs jours d’intervalle et qu’aucun changement de température ou de procédé n’est encore prévu. Une fermentation qui reprend après la mise en bouteille peut produire une pression excessive.

La densité finale et la durée réelle dépendent de la souche, du moût et de la température. Pour une bière acidifiée, la mesure du pH peut aussi aider à suivre le résultat, mais elle ne remplace pas le suivi de la densité pour confirmer la fin de fermentation.

## Points encore inconnus

- température réelle de fermentation;
- moment et fréquence habituels des mesures de densité;
- éventuels changements de température pendant les 30 jours;
- souche utilisée, lorsque la recette n’est pas encore décidée.

Ces détails ne sont pas nécessaires pour sélectionner **Single Stage** si le procédé demeure une phase sans changement planifié, mais ils aideront à affiner les profils BeerSmith et les recommandations de fermentation.
