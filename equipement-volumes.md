# Équipement et planification des volumes

La capacité des cuves détermine la taille des brassins possibles. Il faut planifier les volumes d’eau et de moût depuis le volume visé en fermenteur, tout en respectant la capacité de travail réelle du chaudron et de la cuve d’empâtage.

## Équipement connu

Compréhension actuelle du montage : le chaudron de 32 qt sert à l’ébullition, et la glacière Igloo de 19 L sert de cuve d’empâtage. Cette distinction reste à confirmer puisque le terme « chaudron » peut désigner les deux cuves. La priorité de planification est d’éviter tout débordement.

| Équipement | Capacité connue | À confirmer ou mesurer |
|---|---:|---|
| Chaudron utilisé pour l’ébullition | 32 qt US (≈ 30,3 L); valeur donnée par l’utilisateur comme maximum sans risque | Confirmer si 32 qt est la capacité jusqu’au bord ou un volume de travail sécuritaire vérifié à l’ébullition |
| Cuve d’empâtage / chaudron | Glacière Igloo de 19 L | Mesurer le volume réellement utilisable avec la mouture, jusqu’au niveau sécuritaire de remplissage |

Le chaudron a été acheté chez Mout International, au Canada; l’utilisateur confirme qu’il s’agit de **32 quarts US**, soit environ **30,3 L**, et donne cette valeur comme maximum sans risque. Pour éviter tout débordement, retenir une distinction stricte entre cette limite déclarée et la capacité physique jusqu’au bord. Si 32 qt correspond à la capacité nominale jusqu’au bord plutôt qu’à un niveau de remplissage validé pendant une ébullition, le volume de travail sécuritaire est inférieur et reste à établir. À titre de comparaison, 32 quarts impériaux correspondraient à environ 36,4 L.

## La limite du chaudron

Le volume maximal de travail doit être mesuré et consigné séparément de la capacité nominale. Puisque l’objectif est d’éviter tout débordement, ne pas remplir jusqu’au maximum théorique : conserver une marge libre validée pour l’échauffement, le hot break, l’ébullition active, la mousse et les ajouts. La marge dépend de la forme du chaudron et du comportement du moût; ne pas lui attribuer un pourcentage arbitraire.

Pour établir cette limite :

1. Vérifier si les 32 qt correspondent à la capacité nominale jusqu’au bord ou à un niveau d’ébullition sécuritaire déjà établi.
2. Mesurer les volumes avec un récipient gradué et marquer un niveau de remplissage qui conserve une marge libre réelle.
3. Valider le niveau avec prudence pendant une ébullition représentative, en tenant compte de la montée en température, du hot break, de l’ébullition active et des ajouts; ne jamais tester en remplissant au bord.
4. Consigner le volume maximal de travail validé en litres. Utiliser cette valeur avec sa marge, et non la capacité nominale, pour planifier les brassins.

La valeur déclarée par l’utilisateur est de **32 qt US (environ 30,3 L)**. Tant qu’il n’est pas confirmé qu’il s’agit d’un volume de travail validé avec marge libre, le volume sécuritaire réel doit être considéré comme **non établi**. Ne pas conclure qu’un volume inférieur à 30,3 L est automatiquement sûr.

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

Si le volume pré-ébullition calculé dépasse le volume maximal de travail validé avec marge, le brassin ne tient pas dans la configuration prévue. Même s’il est inférieur à la capacité nominale, ne pas le considérer sûr si la marge de tête n’est pas établie. Ajuster la taille du brassin ou définir explicitement une autre méthode avant de commencer.

## Paramètres à renseigner dans BeerSmith

Le profil d’équipement BeerSmith devrait refléter les mesures de ce système, notamment :

- capacité utile du chaudron et volume d’ébullition;
- taux d’évaporation mesuré pendant une durée d’ébullition connue;
- pertes vers le trub et pendant le transfert;
- volume visé à l’étape définie comme volume de brassin;
- capacité utile de la cuve d’empâtage et son volume mort;
- absorption du grain observée avec le procédé utilisé.

Les noms exacts des champs peuvent varier selon la version et le profil BeerSmith. Après chaque brassin, noter les volumes mesurés aux étapes importantes et mettre à jour le profil.

## Efficacité de brassage provisoire

L’utilisateur ne maîtrise pas encore complètement les performances de son équipement et n’a pas établi son efficacité réelle. En attendant de recueillir assez de données, utiliser **72 % de brew efficiency** comme hypothèse par défaut lorsqu’une recette ne fournit pas d’autre valeur. Ce pourcentage est provisoire : il ne s’agit ni d’une mesure confirmée ni d’une garantie de rendement.

Si une capture d’écran ou les paramètres BeerSmith de la recette indiquent une autre efficacité, utiliser cette valeur pour analyser la recette concernée et signaler qu’elle diffère de l’hypothèse provisoire de 72 %. Ne pas la remplacer silencieusement par 72 % et ne pas traiter une valeur affichée dans une seule recette comme le rendement réel permanent de l’équipement.

Pour affiner le rendement avec l’expérience, conserver après chaque brassin les paramètres BeerSmith utilisés et les mesures réelles pertinentes, notamment la masse et la composition des grains, le volume de moût au point de mesure utilisé par BeerSmith et sa densité initiale. Comparer plusieurs brassins réalisés avec un procédé et des mesures cohérents avant de mettre à jour le profil d’équipement.

## Mesures à compléter

- [ ] Confirmer si 32 qt US (environ 30,3 L) est la capacité jusqu’au bord ou le volume de travail sécuritaire.
- [ ] Mesurer, valider et marquer un niveau maximal de travail qui conserve une marge libre suffisante pour l’ébullition; ne pas utiliser la capacité nominale comme cible.
- [ ] Mesurer le volume de maische maximal que la glacière de 19 L peut contenir tout en permettant de mélanger sans débordement.
- [ ] Mesurer l’évaporation, les pertes de transfert et de trub, le volume mort et l’absorption du grain.
- [ ] Consigner les volumes, densités, moutures et paramètres BeerSmith de plusieurs brassins afin d’estimer et de mettre à jour l’efficacité réelle; conserver 72 % comme hypothèse tant qu’elle n’est pas mieux établie.
- [ ] Définir précisément le volume cible en fermenteur.
- [ ] Calculer le ratio d’empâtage et les volumes de batch sparge pour une recette donnée, en vérifiant la capacité de chaque cuve à chaque étape.
