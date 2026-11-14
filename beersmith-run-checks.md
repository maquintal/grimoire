# Interpréter les alertes Run Checks de BeerSmith

Les messages **Run Checks** signalent des écarts entre les données de la recette et les modèles ou plages configurés dans BeerSmith. Ce sont des pistes à examiner, pas toujours des corrections à appliquer telles quelles.

## Alerte de quantité de levure ou de starter

BeerSmith peut comparer le nombre de cellules estimé pour les emballages affectés à la recette au nombre de cellules demandé par son modèle de taux d’ensemencement. Cette estimation dépend notamment de la fiche de levure, du format de l’emballage, de sa viabilité, du volume et de la densité du moût.

Pour une levure sèche, vérifier la dose recommandée par le fabricant en plus du décompte de cellules de BeerSmith. Le conseil de créer un starter n’est pas automatiquement approprié : ne pas ajouter un starter uniquement pour faire disparaître l’alerte sans vérifier les instructions du fabricant et la configuration de la levure dans BeerSmith.

### Application à la Lichtenhainer actuelle

La capture affiche un lot de **22 L**, une densité initiale de **1,038** (environ 9,5 °P) et un emballage de **11 g de WildBrew Philly Sour**. BeerSmith avertit que la quantité n’atteint pas son besoin estimé de **157,98 milliards de cellules**.

Lallemand indique pour un moût sous 14 °P une dose de **50–100 g/hL**. Pour 22 L, cela correspond à **11–22 g**. Un sachet de 11 g donne 50 g/hL, soit le bas de la plage fabricant; deux sachets donnent 100 g/hL, soit le haut. Ainsi, l’alerte de BeerSmith et la dose fabricant expriment deux modèles différents. Un sachet est à la dose minimale publiée par Lallemand; deux sachets restent dans sa plage si l’on veut davantage de marge. Cette comparaison suppose que les 22 L sont le volume réellement ensemencé et que le sachet contient bien 11 g.

Avant de trancher, vérifier que la fiche BeerSmith correspond bien à de la Philly Sour sèche et au bon format de sachet. Suivre la notice du produit pour son utilisation. La décision entre une dose minimale et une dose supérieure doit aussi tenir compte du procédé et de la souche; le message « add a starter » seul ne permet pas de choisir.

## Alerte de pH d’empâtage

Une alerte indiquant que le pH ajusté ne correspond pas à la cible ne dit pas, à elle seule, si le pH est trop haut ou trop bas, ni quel ajout ferait la correction appropriée.

Avant de modifier l’eau ou la recette, relever :

- le pH cible et le pH calculé après ajustements;
- le profil de l’eau (au minimum les informations saisies dans BeerSmith sur son alcalinité et ses minéraux);
- la quantité et le type d’acide ou de malt acidulé déjà inclus;
- la composition de la mouture et, si possible, une mesure réelle du pH d’empâtage.

Ne pas ajouter automatiquement de malt acidulé ou d’acide sans connaître le sens et l’ampleur de l’écart. Le pH d’empâtage concerne l’empâtage; il n’est pas le pH final de la bière. Une levure acidifiante comme Philly Sour peut produire de l’acide pendant la fermentation, mais ne corrige pas le pH d’empâtage.

Dans la recette actuelle, le malt acidulé représente **7,5 % de la mouture**. L’alerte ne permet pas de conclure s’il faut en ajouter, en retirer ou ajuster l’eau : il faut d’abord voir les valeurs de pH et le profil d’eau dans les onglets **Mash** et **Water**.

## Suggestion de couleur hors plage

BeerSmith estime la couleur à partir des informations de la fiche des malts et de la recette, puis la compare à la plage du style sélectionné. Une suggestion de correction n’est pas en soi la preuve que la bière aura une couleur inappropriée; les fiches de malt et les modèles de couleur sont des estimations.

Dans la capture actuelle, la couleur est estimée à **5,1 EBC**, contre une plage BeerSmith de **5,9–11,8 EBC**. L’écart au minimum est de **0,8 EBC**. Il est faible et ne justifie pas, à lui seul, d’ajouter un malt plus foncé qui pourrait changer le goût. Vérifier la couleur déclarée des malts et les caractéristiques visuelles recherchées avant de modifier la mouture.

## Règle de décision

Pour chaque message **Run Checks** :

1. repérer la valeur concernée, la cible et les données de recette qui la déterminent;
2. vérifier que le profil BeerSmith et les fiches d’ingrédients correspondent au matériel et aux produits réels;
3. comparer avec les consignes du fabricant ou l’objectif sensoriel de la recette;
4. corriger uniquement si l’écart est réel et que la modification ne compromet pas un autre objectif;
5. noter les incertitudes si une donnée indispensable manque, plutôt que de proposer une correction spéculative.

## Référence fabricant

- [Lallemand — WildBrew Philly Sour](https://www.lallemandbrewing.com/en/united-states/products/wildbrew-philly-sour/)
