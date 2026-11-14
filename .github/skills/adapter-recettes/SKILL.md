---
name: adapter-recettes
description: Analyse et adapte des recettes de bière maison pour BeerSmith, l’équipement et les ingrédients réellement disponibles. À utiliser pour résoudre les problèmes de capacité, remplacer un ingrédient ou optimiser une recette sans se limiter à une mise à l’échelle mathématique.
---

# Adapter une recette de bière maison

## Contexte du dépôt à consulter

Avant de proposer une adaptation, lire les fichiers pertinents du dépôt. Les chemins ci-dessous sont relatifs à ce fichier :

- `../../../adapter-recettes.md` — méthode d’analyse et format de réponse attendus;
- `../../../fermentation.md` — procédé de fermentation de l’utilisateur et interprétation des profils BeerSmith;
- `../../../equipement-volumes.md` — équipement connu, contraintes de volumes et mesures encore inconnues;
- `../../../houblons.md` — à consulter pour remplacer un houblon ou recalculer une addition d’amertume;
- `../../../malts.md` — à consulter pour remplacer un malt selon sa fonction, son caractère et son rôle dans l’empâtage;
- `../../../levures.md` — inventaire des levures disponibles;
- `../../../beersmith-yeast.md` — à consulter si la recette implique le calcul ou le choix de levure;
- `../../../beersmith-run-checks.md` — à consulter pour interpréter les alertes générées par BeerSmith;
- `../../../lichtenhainer/remplacer-wlp677-lichtenhainer.md` — à consulter pour Lactobacillus, WLP677, Philly Sour ou une Lichtenhainer.
- `../../../lichtenhainer/optimisation-lichtenhainer.md` — à consulter pour analyser la recette Lichtenhainer visible dans BeerSmith.

Consulter le README et d’autres documents du dépôt si la question touche un sujet qui y est répertorié. Ne pas supposer qu’une capture ou un profil BeerSmith est plus à jour que les contraintes réelles consignées par l’utilisateur.

## Contraintes connues à garder en tête

- Le chaudron est de 32 qt US (environ 30,3 L). L’utilisateur indique cette valeur comme maximum sans risque, mais il faut distinguer un niveau d’utilisation validé à l’ébullition de la capacité jusqu’au bord. Ne jamais recommander de remplir le chaudron à sa capacité nominale.
- La cuve d’empâtage réelle est une glacière Igloo de 19 L. Sa capacité utile avec le grain et l’espace nécessaire au mélange reste à mesurer.
- L’utilisateur ne maîtrise pas encore complètement les performances de son équipement. En l’absence d’une autre valeur dans les informations fournies pour une recette, utiliser **72 % de brew efficiency** comme hypothèse provisoire, pas comme rendement mesuré. Si une capture d’écran indique une autre efficacité, utiliser et signaler cette valeur pour la recette concernée plutôt que de la remplacer par 72 %.
- Le batch sparging peut répartir les ajouts d’eau de rinçage en plusieurs lots; il n’augmente ni la capacité de la cuve d’empâtage ni celle du chaudron.
- La priorité explicite de l’utilisateur est d’éviter tout débordement. Ne jamais optimiser le volume au plus près de la capacité nominale; conserver une marge libre validée pour le chauffage, l’ébullition, la mousse et les ajouts.
- Vérifier toute différence entre la configuration d’équipement BeerSmith et l’équipement réel. Une capture de recette a montré un profil « Cooler 5gal (21L) », alors que la cuve réelle documentée est de 19 L : ne pas considérer ces valeurs comme équivalentes sans confirmation.
- WildBrew Philly Sour est une levure acidifiante, pas une culture de Lactobacillus. Pour une culture bactérienne ou une fermentation mixte, tenir compte des différences décrites dans le document consacré à WLP677.
- Le procédé actuel de l’utilisateur est une fermentation en un seul fermenteur, suivie d’environ 30 jours avant l’embouteillage. Le profil BeerSmith **Single Stage** convient si aucune seconde phase distincte n’est prévue. Ne pas traiter 30 jours comme preuve de fermentation terminée; vérifier la stabilité de la densité avant embouteillage.
- Les messages **Run Checks** sont des alertes à diagnostiquer, pas des instructions à suivre automatiquement. Pour une levure sèche, comparer le modèle de cellules BeerSmith à la dose fabricant; pour une alerte de pH, ne recommander aucun ajustement sans connaître le pH calculé, la cible et le profil d’eau.

## Procédure

1. **Lire la recette comme un procédé complet.** Extraire de la recette ou des captures les ingrédients, quantités, volume de brassin, volume pré-ébullition, efficacité de brassage, étapes d’empâtage/rinçage, ébullition, levures et paramètres BeerSmith. Conserver les unités et distinguer les valeurs entrées des valeurs calculées.
2. **Définir l’intention.** Identifier le style, les caractéristiques sensorielles à préserver et les compromis acceptables. Distinguer les éléments essentiels au caractère de la bière des éléments plus flexibles.
3. **Diagnostiquer le problème.** Déterminer si la recette ne tient pas à cause du volume, d’un profil d’équipement incorrect, de la capacité de la cuve, d’un ingrédient manquant, d’un choix de procédé ou d’un autre paramètre. Ne pas réduire le problème à « changer l’échelle » avant ce diagnostic.
4. **Analyser le rôle de chaque changement envisagé.** Évaluer les ingrédients selon leur fonction et leurs effets sur le goût, la densité, l’amertume, la couleur, le corps et la fermentation. Utiliser les tableaux de `houblons.md` et `malts.md` comme points de départ, puis tenir compte de l’inventaire réel; ne pas présenter une substitution fonctionnelle comme une équivalence exacte.
5. **Comparer des adaptations.** Proposer l’option la plus cohérente et, si cela aide à la décision, une alternative avec ses avantages et compromis. Respecter les méthodes réellement disponibles, notamment le rinçage par lots lorsque pertinent.
6. **Vérifier quantitativement.** Utiliser les calculs pour contrôler les volumes à chaque étape, le volume en fermenteur visé, la capacité des cuves, la densité, l’amertume et la quantité de levure. Une règle de trois peut servir de point de départ, jamais de justification suffisante.
7. **Traiter explicitement les incertitudes.** Séparer les faits confirmés, les estimations et les hypothèses. Si une capacité maximale, un profil BeerSmith ou un paramètre essentiel est inconnu, ne pas inventer de valeur ni déclarer le brassin réalisable sans réserve.

## Points d’attention

- Le volume visé en fermenteur, le volume post-ébullition et le volume pré-ébullition sont différents. Prendre en compte l’évaporation et les pertes mesurées; confirmer le point auquel chaque volume BeerSmith se rapporte.
- Pour prévenir les débordements, comparer le volume pré-ébullition au **volume maximal de travail validé avec une marge de tête**, pas à la capacité nominale. Comparer les volumes sur la même base de température et tenir compte de l’expansion au chauffage, de la mousse/hot break et des ajouts de houblon.
- Ne pas inventer une marge universelle en pourcentage. Si le volume maximal de travail avec marge n’a pas été mesuré ou confirmé, déclarer la sécurité non validée et ne pas recommander de faire bouillir le volume prévu tel quel; proposer de réduire le lot ou d’établir d’abord un niveau de remplissage sûr.
- Dans la capture Lichtenhainer la plus récente, le volume pré-ébullition est de 26,56 L, soit 3,74 L sous les 30,3 L déclarés. Cet écart ne prouve pas l’absence de débordement tant que les 32 qt n’ont pas été confirmés comme limite d’exploitation avec marge libre.
- Pour la cuve d’empâtage, vérifier le volume combiné de l’eau et du grain, ainsi que l’espace nécessaire pour mélanger. Ne pas confondre capacité de la cuve et volume d’eau d’empâtage admissible.
- La mise à l’échelle uniforme ne préserve pas nécessairement les résultats : l’utilisation du houblon, le rendement, les pertes, la capacité d’empâtage et le comportement de la levure peuvent dépendre du volume, de la densité et du procédé. Pour les substitutions de houblon, distinguer les ajouts d’amertume des ajouts aromatiques et recalculer les IBU avec le houblon, le lot et le format réellement disponibles; consulter `houblons.md`.
- Pour la **brew efficiency**, prendre 72 % comme hypothèse provisoire uniquement si la recette ou sa capture ne donne pas une autre valeur. Si une autre valeur est visible, l’utiliser pour analyser cette recette et signaler l’écart avec l’hypothèse provisoire; ne pas en déduire que le rendement réel du système est déjà établi. Mettre à jour l’estimation à partir des mesures consignées lors des brassins.
- L’objectif est d’adapter la recette en préservant au mieux sa fonction et son intention, pas de convertir les ingrédients par une règle de trois. Pour remplacer un houblon ou un malt, comparer les rôles, les effets sensoriels et les contraintes de procédé à l’aide des tableaux de références; utiliser les calculs pour contrôler ou affiner une décision déjà fondée sur ces éléments, jamais comme unique raisonnement.
- Vérifier les calculs de levure avec la bonne souche, le format réel du sachet, le taux d’ensemencement retenu et les recommandations du fabricant. Pour une fermentation acidifiante ou mixte, analyser séparément le rôle de la bactérie et celui de la levure.
- Pour chaque alerte **Run Checks**, expliquer ce que le logiciel mesure et ce qu’il ne mesure pas. Ne pas ajouter automatiquement un starter, un acide ou un malt coloré pour faire disparaître une alerte; consulter `beersmith-run-checks.md` et vérifier la recette, l’équipement et les recommandations applicables.
- Ne pas confondre un profil BeerSmith de fermentation en une ou deux étapes avec le nombre de souches ajoutées. Une attente de plusieurs jours dans un seul fermenteur ne constitue pas à elle seule une seconde étape; vérifier si une phase distincte de température ou de procédé est réellement prévue.
- Consulter `fermentation.md` pour appliquer le procédé actuel. Distinguer une seule étape de fermentation, une période de maturation, un changement de phase/température et le nombre de souches; ne jamais déduire la fin de fermentation du seul nombre de jours.
- Si une capture révèle une discordance entre BeerSmith et l’équipement ou les autres données connues, la signaler avant d’optimiser les quantités. Ne pas modifier silencieusement le profil d’équipement supposé.

## Présentation de la réponse

Structurer la réponse autour de :

1. **Diagnostic** — ce qui ne fonctionne pas et pourquoi;
2. **Intention à préserver** — style et caractéristiques clés;
3. **Adaptation proposée** — changements et justification;
4. **Contrôles BeerSmith et équipement** — résultats des calculs et limites;
5. **Compromis et incertitudes** — différence attendue, données à confirmer et degré de confiance.

Poser une question seulement lorsque la réponse peut changer sensiblement le choix de procédé ou l’adaptation. Sinon, énoncer clairement une hypothèse raisonnable et fournir une proposition conditionnelle.
