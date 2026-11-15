# Adaptation de la Kölsch fumée

Cette référence porte sur la [recette Kölsch Fumée d’Univers Bière](https://univers-biere.net/rec_kolsch_fumee.php), en particulier sur le remplacement du houblon expérimental Cophoudal GR50.

## Style à préserver

La recette source décrit une **Kölsch fumée**. Si la fumée est la seule différence spéciale, le repère BJCP 2021 est **32A. Classic Style Smoked Beer**, avec la **Kölsch (5B)** comme style de base à préciser. La catégorie 32B peut être pertinente si le houblon expérimental GR50 est considéré comme un ingrédient spécial supplémentaire qui transforme la bière en une création plus unique; le choix dépend aussi de l’objectif (brassage maison ou compétition). Dans tous les cas, préserver le caractère de base Kölsch et l’équilibre agréable de la fumée avec les notes du houblon. Voir [Choisir un guide de style](../styles-biere.md).

## Remplacer la levure WLP029

La recette source (23 L, OG estimée 1,046) demande un emballage de **German Ale/Kölsch WLP029**. Le meilleur substitut de l’inventaire documenté est **SafAle K-97** : Fermentis la recommande notamment pour les Kölsch délicates et décrit une fermentation subtile, florale et modérément fruitée. C’est une souche différente, mais elle est plus cohérente avec le caractère Kölsch qu’une levure anglaise ou une levure neutre générique.

**Dose de départ : un sachet de K-97 de 11,5 g** pour les 23 L de la recette, si le format acheté est bien 11,5 g. Fermentis recommande 50–80 g/hl, soit 11,5–18,4 g pour 23 L; un sachet de 11,5 g correspond donc au bas de la plage. L’emballage liquide de WLP029 affiché par BeerSmith (`1,0 pkg`, 35,49 ml) ne se convertit pas en un sachet sec par simple égalité du nombre d’emballages. Vérifier le poids sur le sachet et configurer K-97 avec son format réel dans BeerSmith.

La fiche Fermentis indique une atténuation apparente de 80–84 %, une sédimentation lente et une plage de fermentation idéale de 18–26 °C. Le résultat peut être un peu plus sec et la clarification plus lente; si le contrôle de température le permet, viser le bas de la plage fabricant pour garder un profil délicat. Suivre la densité jusqu’à sa stabilité avant l’embouteillage.

Source fabricant : [Fermentis — SafAle K-97](https://fermentis.com/en/product/safale-k-97/).

### Lecture de la capture BeerSmith Yeast

La capture montre un taux choisi et recommandé de **0,75 million de cellules/ml/°P**, dans une plage affichée de **0,35–1,15**. BeerSmith calcule **202,4 milliards** de cellules nécessaires. La ligne « SafAle German Ale » indique **125,69 milliards** de cellules viables pour un sachet (viabilité **94,72 %**).

Les **8,80 millions de cellules/ml** affichés sont la concentration cible, pas la concentration apportée par le sachet. Sur 23 L, le sachet fournit environ **5,46 millions/ml**, soit **62 %** de la cible; le quotient est **1,61 sachet**, donc deux sachets seraient nécessaires pour atteindre ou dépasser strictement 0,75. Deux apporteraient environ **251 milliards** de cellules (124 % de la cible) et un taux estimé d’environ **0,93**, toujours dans la plage affichée. Un sachet correspond à environ **0,47**, lui aussi dans la plage, mais sous le taux recommandé.

**Décision pour cette recette : un sachet K-97 de 11,5 g**, si c’est bien le poids sur le produit acheté. À 23 L, cela correspond à **50 g/hl**, le bas de la dose fabricant Fermentis (50–80 g/hl). Deux sachets (23 g, soit 100 g/hl) dépasseraient cette dose fabricant; ne pas en mettre deux uniquement pour atteindre le chiffre calculé par BeerSmith.

La capture utilise la fiche générique **SafAle German Ale**, pas une fiche nommée K-97. Avant le brassage, sélectionner la fiche K-97 si disponible, ou vérifier manuellement que le poids et les cellules par sachet correspondent au produit réel. La décision d’un sachet suit ici le dosage fabricant et reste dans la plage d’ensemencement affichée; le démarrage peut être un peu plus lent qu’au taux recommandé par BeerSmith. Suivre la fermentation et vérifier la stabilité de la densité avant l’embouteillage.

## Remplacer le GR50

La recette source (23 L) utilise **20 g de GR50 à 6 % à 10 minutes** (5,3 IBU) et **30 g à 5 minutes** (4,3 IBU). Le GR50 est décrit comme un croisement de Cascade et Strisselspalt, avec des notes de melon, citron, fruits exotiques et une touche épicée. Ces ajouts tardifs contribuent à la saveur et à l’arôme, pas seulement à l’amertume.

Le meilleur remplacement dépend des houblons réellement disponibles :

- **Cascade**, si disponible, est le choix simple le plus proche pour les notes fruitées et d’agrumes, mais il préservera moins le côté épicé/noble du GR50.
- Pour mieux couvrir les deux facettes, combiner un houblon fruité/agrumé (par exemple Cascade) et un houblon noble légèrement épicé (par exemple Strisselspalt, Tettnang ou Saaz), si ces variétés sont disponibles. Ajuster le mélange selon les fiches et les quantités réelles, plutôt que d’imposer une proportion universelle.
- **Brewer’s Gold**, présent dans une recette BeerSmith déjà examinée, est une solution de repli conditionnelle si ce houblon est encore physiquement disponible. Il apportera un fruité plus marqué, souvent plus proche des fruits rouges/baies que du melon-citron; ce n’est pas un équivalent du GR50.

### Proposition de départ

Si **Cascade** est disponible et que son lot est proche de **6 % d’acides alpha**, remplacer le GR50 par **20 g de Cascade à 10 minutes** et **30 g à 5 minutes**. Garder l’ajout de Magnum à 80 minutes inchangé. Cela devrait fournir une amertume estimée proche des **5,3 et 4,3 IBU** de la source, mais donnera un profil plus citronné/agrumé, moins melon et épicé.

Si le Cascade disponible a un pourcentage d’acides alpha différent, entrer sa valeur d’étiquette dans BeerSmith et ajuster les grammes pour retrouver environ **5,3 IBU à 10 minutes** et **4,3 IBU à 5 minutes**. L’équivalence d’IBU ne garantit pas une intensité aromatique identique; goûter et tenir compte du profil du lot.

La présence d’une variété dans une recette ou dans la base BeerSmith ne confirme pas son stock physique. L’inventaire réel des houblons disponibles n’étant pas consigné ici, Cascade et les autres options restent conditionnelles.
