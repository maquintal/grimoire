# Équipement et planification des volumes

La capacité des cuves détermine la taille des brassins possibles. Il faut planifier les volumes d’eau et de moût depuis le volume visé en fermenteur, tout en respectant la capacité de travail réelle du chaudron et de la cuve d’empâtage.

## Équipement connu

Compréhension actuelle du montage : le chaudron de 32 qt sert à l’ébullition, et la glacière Igloo de 19 L sert de cuve d’empâtage. Cette distinction reste à confirmer puisque le terme « chaudron » peut désigner les deux cuves.

| Équipement | Capacité connue | À confirmer ou mesurer |
|---|---:|---|
| Chaudron utilisé pour l’ébullition | 32 qt nominaux, présumés US (≈ 30,3 L) | Vérifier la graduation et mesurer le volume de travail maximal sans débordement |
| Cuve d’empâtage / chaudron | Glacière Igloo de 19 L | Mesurer le volume réellement utilisable avec la mouture, jusqu’au niveau sécuritaire de remplissage |

Le chaudron a été acheté chez Mout International, au Canada; les 32 qt sont donc présumés être des quarts US, soit environ **30,3 L nominaux**. Cette unité reste à confirmer sur la graduation ou la fiche du produit. À titre de comparaison, 32 quarts impériaux correspondraient à environ 36,4 L. Dans les deux cas, la capacité nominale ne donne pas le volume maximal sécuritaire : la capacité jusqu’au bord n’est pas une limite de remplissage à utiliser pendant l’ébullition.

## La limite du chaudron

Le volume maximal de liquide doit être mesuré et consigné séparément de la capacité nominale. Laisser une marge libre pour l’ébullition, la mousse et les ajouts; le niveau sécuritaire dépend de la forme du chaudron et du comportement du moût.

Pour établir cette limite :

1. Vérifier sur la graduation ou la fiche du produit que les 32 qt sont bien des quarts US, puis mesurer la capacité réelle du chaudron avec de l’eau, par volumes connus.
2. Choisir et marquer un niveau de remplissage qui laisse une marge libre suffisante sous le bord.
3. Vérifier ce niveau avec prudence lors d’une ébullition habituelle, sans remplir le chaudron jusqu’au bord.
4. Consigner le niveau maximal retenu en litres. Utiliser cette valeur, et non les 32 qt nominaux, dans les calculs de brassin.

Tant que cette mesure n’est pas faite, le volume maximal sécuritaire est **inconnu**. Il ne faut donc pas conclure que tout volume inférieur à 32 qt est sûr à bouillir.

## Cuve d’empâtage et batch sparging

La glacière Igloo de 19 L sert de cuve d’empâtage. Ses 19 L représentent sa capacité nominale, pas nécessairement le volume d’eau d’empâtage admissible : la cuve contient à la fois l’eau et le grain, et il faut garder de l’espace pour mélanger sans déborder.

Le ratio d’empâtage est le volume d’eau d’empâtage par masse de grain, généralement exprimé en L/kg. Le volume de la maische dépend donc du ratio **et** de la quantité de grain; le ratio seul ne confirme pas que la maische entre dans la glacière.

Le **batch sparging** (rinçage par lots) permet de recueillir le moût en plusieurs étapes : après l’égouttage de l’empâtage, l’eau de rinçage peut être ajoutée et égouttée en plusieurs lots. Cela aide à adapter les ajouts à la capacité de la cuve et permet de répartir les volumes de rinçage; cela n’augmente ni la capacité de la cuve ni celle du chaudron. Le volume total recueilli doit toujours respecter la limite de travail du chaudron avant l’ébullition.

## Du volume en fermenteur au volume d’ébullition

Le volume désiré en fermenteur ne correspond pas au volume à préparer avant l’ébullition. Pour le planifier, tenir compte des pertes et des paramètres réels du système :

- évaporation pendant l’ébullition;
- moût retenu dans le chaudron, les drêches ou le matériel de transfert;
- trub et houblon laissés derrière, selon la méthode de transfert;
- absorption d’eau par le grain et volume mort de la cuve d’empâtage.

En première approximation :

```text
Volume pré-ébullition = volume post-ébullition souhaité + évaporation
Volume d’eau total = volume pré-ébullition + rétention dans le grain + volumes morts
```

Il faut préciser où le volume « souhaité » est mesuré : volume en fermenteur, volume post-ébullition dans le chaudron, ou autre point du procédé. Les pertes de transfert et de trub doivent être ajoutées lorsqu’elles séparent ces points de mesure. Les pertes réelles varient selon le système; il est préférable de les mesurer sur plusieurs brassins plutôt que d’utiliser des valeurs supposées.

Si le volume pré-ébullition calculé dépasse la limite sécuritaire du chaudron, le brassin ne tient pas dans la configuration prévue. Il faut ajuster la taille du brassin ou définir explicitement une autre méthode de brassage avant de commencer.

## Paramètres à renseigner dans BeerSmith

Le profil d’équipement BeerSmith devrait refléter les mesures de ce système, notamment :

- capacité utile du chaudron et volume d’ébullition;
- taux d’évaporation mesuré pendant une durée d’ébullition connue;
- pertes vers le trub et pendant le transfert;
- volume visé à l’étape définie comme volume de brassin;
- capacité utile de la cuve d’empâtage et son volume mort;
- absorption du grain observée avec le procédé utilisé.

Les noms exacts des champs peuvent varier selon la version et le profil BeerSmith. Après chaque brassin, noter les volumes mesurés aux étapes importantes et mettre à jour le profil.

## Mesures à compléter

- [ ] Vérifier sur la graduation ou la fiche du produit que le chaudron de 32 qt est en quarts US (présumé : environ 30,3 L nominaux).
- [ ] Mesurer et marquer son volume maximal de travail sécuritaire pendant l’ébullition.
- [ ] Mesurer le volume de maische maximal que la glacière de 19 L peut contenir tout en permettant de mélanger sans débordement.
- [ ] Mesurer l’évaporation, les pertes de transfert et de trub, le volume mort et l’absorption du grain.
- [ ] Définir précisément le volume cible en fermenteur.
- [ ] Calculer le ratio d’empâtage et les volumes de batch sparge pour une recette donnée, en vérifiant la capacité de chaque cuve à chaque étape.
