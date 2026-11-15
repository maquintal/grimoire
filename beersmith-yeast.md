# Interpréter l’onglet Yeast de BeerSmith

Cette page répond à la première question du dépôt : comment lire l’onglet **Yeast** et estimer la quantité de levure à ajouter. Les valeurs dépendent de la recette, du type de fermentation et des données enregistrées dans la fiche de levure BeerSmith.

## Les principaux champs

- **Pitch Rate** : taux d’ensemencement utilisé par BeerSmith, généralement exprimé en millions de cellules par ml et par degré Plato. Il sert à estimer le nombre de cellules à ensemencer.
- **Recommended Pitch Rate** et **Pitch Rate Range** : repère et plage recommandés par BeerSmith selon ses réglages et le type de fermentation. Ce sont des guides, pas une mesure de la levure réellement viable.
- **Est cells per ml** : concentration cible de cellules par ml calculée selon le **Pitch Rate** sélectionné et la densité du moût. Ce n’est pas nécessairement la concentration que la quantité de levure affectée à la recette fournit réellement.
- **Yeast Cells Needed** : nombre total de cellules que BeerSmith estime nécessaire pour le taux choisi et la recette.
- **Yeast** : levure(s) affectée(s) à la recette. Les dates, la viabilité et le nombre de cellules par emballage proviennent notamment de la fiche de levure et des paramètres saisis.
- **Amount** : quantité affectée à la recette, par exemple `1.0 pkg` pour un emballage. Vérifier la taille et le nombre de cellules configurés dans la fiche BeerSmith : le nom de la levure seul ne garantit pas que la fiche corresponde au sachet acheté.
- **Calculate Viability** : lorsque cette option est activée, BeerSmith estime la viabilité selon la date et son modèle de vieillissement. Cette estimation n’est pas une analyse de laboratoire; elle dépend aussi de l’exactitude de la date, de la fiche et des conditions de conservation.
- **Yeast Cells Without Starter** : estimation des cellules viables apportées sans starter. Un starter peut augmenter la quantité de cellules, mais n’est pas automatiquement nécessaire pour chaque levure ou chaque recette.
- **Dry Yeast Hydration** : paramètres de réhydratation de levure sèche. Suivre en priorité les consignes du fabricant de la levure utilisée.
- **Use Two Stage Yeast Starter** et **Use Stir Plate** : options liées au calcul d’un starter en une ou deux étapes et à l’utilisation d’un agitateur.

## Onglet Yeast et profil de fermentation

La liste des souches dans l’onglet **Yeast** et le profil **Fermentation** sont deux réglages distincts. Avoir deux levures dans la recette ne signifie pas que le profil doit être « Two Stage »; de même, un profil « Two Stage » ne signifie pas qu’il faut ajouter deux levures.

Le choix **Single Stage** correspond au procédé décrit dans [Fermentation](fermentation.md) lorsqu’une seule phase est prévue. Une seconde phase de température ou de procédé peut justifier un profil à plusieurs étapes, même si la bière reste dans le même fermenteur. La durée totale, à elle seule, ne détermine pas le nombre d’étapes.

## Lecture de la capture d’écran

La recette affiche un **Pitch Rate** de `0,75`, tandis que BeerSmith affiche une recommandation de `1,50` et une plage de `1,10–1,90`. Cela indique que le taux choisi est inférieur au repère affiché.

Pour la LalBrew NovaLager, la capture montre une quantité de `1,0 pkg`, une viabilité estimée de `95,20 %` et `157,08 milliards` de cellules viables. Le total **Yeast Cells Without Starter** est aussi de `157,1 milliards`. Une autre ligne de levure affiche `0,0 pkg` et `0,00 milliard` : elle ne contribue donc pas au total indiqué.

BeerSmith affiche `196,1 milliards` de **Yeast Cells Needed**. En comparant seulement ces deux nombres :

```text
196,1 milliards nécessaires ÷ 157,08 milliards par sachet ≈ 1,25 sachet
```

Selon les données de cette fiche BeerSmith, un sachet ne suffit pas à atteindre les `196,1 milliards`; deux sachets entiers dépasseraient ce total. C’est une estimation conditionnelle : elle suppose que la fiche BeerSmith correspond bien au sachet de NovaLager acheté et que les cellules viables par sachet sont correctement configurées.

### Point à vérifier dans cette capture

Les chiffres méritent une vérification avant de conclure que deux sachets sont la quantité définitive. `157,08` milliards représente environ 80 % de `196,1` milliards, alors que le taux affiché (`0,75`) représente la moitié du taux recommandé (`1,50`). Ces proportions ne concordent pas directement.

Vérifier dans BeerSmith :

1. le volume de moût et sa densité initiale (ou son degré Plato);
2. le type de fermentation et le taux d’ensemencement choisi;
3. la taille du sachet et le nombre de cellules configurés dans la fiche LalBrew NovaLager;
4. les dates, la viabilité et les quantités affectées à la recette.

Le calcul du nombre de sachets ne doit pas reposer sur le seul champ **Amount**. Il faut d’abord confirmer le besoin total en cellules et la contribution réaliste d’un emballage.

## Méthode de calcul

Quand BeerSmith donne un besoin en cellules et un nombre de cellules viables par emballage :

```text
Nombre théorique d’emballages =
    cellules nécessaires ÷ cellules viables par emballage
```

Pour des sachets vendus en unités entières, arrondir le résultat vers le haut, puis vérifier que les paramètres de la fiche BeerSmith correspondent à l’étiquette et aux consignes du fabricant. Pour une levure sèche, les recommandations du fabricant (par exemple une dose en grammes selon le volume) constituent aussi une méthode utile; ne pas mélanger arbitrairement une dose en grammes et une estimation en cellules.

Le besoin en cellules varie avec le volume de moût, sa densité, le taux d’ensemencement retenu et la souche. Le nombre de sachets n’est donc pas une constante attachée à la recette ou à la souche seule.

## Interpréter une capture et choisir le nombre de sachets

Pour répondre à « combien de sachets? », ne pas lire isolément le nombre **Yeast Cells Needed**. Relever et comparer :

1. volume et densité initiale du moût;
2. **Pitch Rate** sélectionné, **Recommended Pitch Rate** et **Pitch Rate Range**;
3. **Yeast Cells Needed**;
4. cellules viables et quantité par emballage, en vérifiant que la fiche correspond à la souche et au format réellement acheté;
5. pour une levure sèche, poids du sachet et dosage massique recommandé par le fabricant.

Le calcul BeerSmith indique la quantité nécessaire selon le taux d’ensemencement sélectionné. Le nombre réellement apporté par les sachets peut toutefois rester dans la plage affichée sans atteindre le taux recommandé. Une fiche générique ou un nombre de cellules par emballage inexact peut aussi créer un écart. Comparer ce résultat aux consignes de dosage du fabricant pour la souche sèche concernée; ne pas mélanger arbitrairement cellules calculées et grammes.

Présenter clairement les deux lectures si elles divergent, puis choisir et justifier une dose. Pour des sachets entiers, le quotient « cellules nécessaires / cellules viables par sachet » est une estimation, pas une consigne automatique d’arrondir vers le haut : vérifier le taux correspondant à la dose entière, le dosage fabricant et la pertinence de la fiche. Ne modifier le **Pitch Rate** que pour exprimer une cible réellement retenue, pas seulement pour faire disparaître un avertissement.

### Conséquences d’une dose trop basse ou trop élevée

- **Sous-ensemencement marqué** : démarrage plus lent, fermentation prolongée ou incomplète et risque accru de stress ou de caractères fermentaires indésirables. Un résultat sous le taux recommandé par BeerSmith n’est pas automatiquement un sous-ensemencement problématique si la dose respecte les consignes du fabricant et demeure dans une plage acceptable.
- **Sur-ensemencement marqué** : généralement pas un danger pour la personne qui boit la bière, mais peut réduire la croissance et la contribution aromatique de la levure, modifier le profil final et gaspiller du produit. Une dose au-dessus de la plage fabricant doit être justifiée par une raison concrète, pas seulement par l’arrondi de BeerSmith.

## Est-ce dangereux d’en mettre trop?

Dans les quantités habituelles du brassage maison, dépasser un peu la quantité cible n’est généralement pas un danger pour la personne qui boit la bière. Le principal enjeu est plutôt le résultat : un ensemencement trop élevé peut modifier le profil de fermentation (notamment les arômes produits par la levure), réduire la croissance de la levure et gaspiller des sachets. L’effet dépend de la souche, du style et du procédé; il n’existe pas ici de seuil universel permettant de déclarer qu’un sachet de plus est toujours sans conséquence.

À l’inverse, un ensemencement trop faible peut ralentir ou stresser la fermentation et nuire au résultat. L’objectif est donc de viser une quantité cohérente avec la recette et les recommandations de la souche, pas d’ajouter le plus de levure possible.

## À préciser pour calculer les prochaines recettes

Pour déterminer le nombre de sachets d’une recette donnée, noter :

- le volume de moût à ensemencer;
- la densité initiale (ou le degré Plato);
- le style et le type de fermentation (ale ou lager, par exemple);
- la souche, le format du sachet et sa date;
- les cellules viables ou la dose recommandée par le fabricant;
- le taux d’ensemencement choisi dans BeerSmith.
