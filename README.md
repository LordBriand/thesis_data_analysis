
# Analyse de la contamination des sources d'eau par des Bactéries Gram Négatives (BGN)

## Description du projet

Ce projet vise à analyser sous R les facteurs influençant la contamination des sources d'eau par des Bactéries Gram Négatives (BGN) dans les villages de Lama-bas (Kara, TOGO). L'étude examine plusieurs variables, notamment la présence de dépotoirs, de latrines, la couverture des puits, et les pratiques de contrôle qualité, la nature des sources d'eau, l'usage faite de l'eau etc...

## Objectifs

- Évaluer l'influence de divers facteurs environnementaux et comportementales sur la contamination par BGN
- Identifier les pratiques potentiellement protectrices contre la contamination
- Fournir des recommandations pour améliorer la gestion des ressources en eau

## Données

Les données utilisées dans cette analyse proviennent de d'un sondage realisée dans 4 villages du canton de Lama à Kara, en Aout 2022. Le jeu de données comprend 38 observations et 26 variables.

## Méthodologie

L'analyse statistique inclut :
- Calcul des Odds Ratios et intervalles de confiance
- Tests du Chi-carré
- Tests exacts de Fisher (pour les petits échantillons)

## Structure du projet

```
projet/
│   README.md
|   associated_factors_GNB.html   (fichier html contenant le rendu du fichier R markdown)
│   script_analyse.R   (à venir)
│   associated_factors_GNB.Rmd   (rapport R markdown des analyses pour la recherche des facteurs associes au portage de BGN)
│
└───data/
│   │   dataframe_these_Briand.csv 
└───

```

## Packages R utilisés

- Epi
- dplyr
- knitr
- kableExtra
- ggplot2
-

## Résultats principaux

  -Influence de la présence de dépotoirs :

Odds Ratio (OR) : 4,1176 [IC 95% : 0,4294 - 39,4817]
Aucune association significative n'a été trouvée entre la présence de dépotoirs et la contamination par BGN (p-value = 0,397).


  -Influence de la présence de latrines :

OR : 1,7500 [IC 95% : 0,2746 - 11,1519]
Aucune association significative n'a été observée entre la présence de latrines et la contamination par BGN (p-value = 0,9014).


  -Influence de la couverture des puits :

OR : 1,0286 [IC 95% : 0,1986 - 5,3262]
Aucune association significative n'a été trouvée entre la couverture des puits et la contamination par BGN (p-value = 1,0000).


  -Influence du contrôle qualité en début d'utilisation :

OR : 3,2000 [IC 95% : 0,4921 - 20,8094]
Une tendance non significative a été observée, suggérant que l'absence de contrôle qualité initial pourrait être associée à un risque accru de contamination par BGN (p-value = 0,4244).


## Limites et perspectives

**Limites :**

-Taille d'échantillon limitée : La plupart des analyses souffrent d'un manque de puissance statistique dû à un petit nombre d'observations.
-Largeur des intervalles de confiance : Les estimations des OR ont des intervalles de confiance très larges, indiquant une grande incertitude.
-Applicabilité limitée du test du Chi-carré : Pour plusieurs analyses, l'approximation du Chi-carré pourrait ne pas être fiable en raison de la petite taille de l'échantillon.
-Analyse bivariée : L'étude n'a pas pris en compte les effets combinés de multiples facteurs sur la contamination par BGN.

**Perspectives :**

-Augmentation de la taille de l'échantillon : Réaliser une étude à plus grande échelle pour améliorer la précision des estimations et la puissance statistique.
-Analyse multivariée : Examiner simultanément l'influence de plusieurs facteurs sur la contamination par BGN pour tenir compte des interactions potentielles.
-Étude longitudinale : Suivre l'évolution de la contamination au fil du temps pour mieux comprendre les facteurs de risque à long terme.
-Exploration de facteurs additionnels : Inclure d'autres variables potentiellement influentes comme les caractéristiques du sol, ou les pratiques d'entretien...
-Amélioration des méthodes de mesure : Développer des protocoles plus précis pour évaluer la qualité de la couverture des puits et l'efficacité des contrôles qualité.
-Étude des mécanismes : Approfondir la compréhension des mécanismes par lesquels certains facteurs pourraient influencer la contamination bactérienne.
-Évaluation des interventions : Tester l'efficacité de différentes interventions (comme l'amélioration des couvertures de puits ou des protocoles de contrôle qualité) dans un cadre expérimental.

Ces résultats et perspectives soulignent l'importance de poursuivre les recherches pour mieux comprendre et prévenir la contamination des sources d'eau par les BGN, avec une attention particulière à la méthodologie et à la taille des échantillons dans les futures études.



## Comment utiliser ce projet ?

1. Clonez ce dépôt
2. Installez les packages R nécessaires
3. Exécutez le script d'analyse ou générez le rapport final

## Auteur

Briand AWIDEYA, PharmD student

## Licence

Ce projet n'est soumis à aucune licence .

## Remerciements

Je voudrais exprimer ma gratitude à :
  -Mon partenaire Dr David ATOKOU qui m'a aidé dans toutes les etapes de la realisation de ce projet : de la collecte des donnees a la redaction en passant par l'analyse des donnees.

