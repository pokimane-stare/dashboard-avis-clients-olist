# Dashboard Power BI : avis clients, ventes et vendeurs

Analyse de la satisfaction des clients d'une place de marché en ligne et de son lien avec les ventes, les annulations et la performance des vendeurs.

## Objectif
Comprendre ce qui influence la note des avis clients et mesurer l'impact de la satisfaction sur le chiffre d'affaires et les annulations de commandes.

## Données
- Jeu de données : [ Brazilian E-Commerce (Olist)] – (https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)]
- 9 tables : clients, commandes, articles commandés, paiements, avis, produits, catégories de produits, vendeurs, géolocalisation.
- Les données ont été chargées dans Snowflake, puis connectées à Power BI.

## Indicateurs clés
| Indicateur | Valeur |
|---|---|
| Nombre d'avis | 99 000 |
| Note moyenne des vendeurs | 4,09 |
| Avis négatifs | 15 000 (14,69 %) |
| Avis positifs | 77,07 % |
| Taux d'annulation | 0,63 % (625 commandes) |
| Ventes totales | 13,59 M |

## Ce que montre le dashboard
- Évolution des avis positifs et négatifs par année, trimestre, mois et jour (2017 à 2018)
- Taux d'annulation selon la note de l'avis
- Ventes et nombre de commandes selon la note de l'avis
- Les 5 catégories de produits les mieux notées
- Note, ventes et commandes par vendeur

## Résultats clés
- Les commandes notées 1 étoile ont le taux d'annulation le plus élevé (environ 4 %), alors que les commandes notées 5 étoiles en ont un très faible.
- Les commandes notées 5 étoiles génèrent la plus grande part des ventes (environ 7,7 M sur 13,59 M).
- Le nombre d'avis augmente fortement entre 2017 et 2018, avec des pics ponctuels.
- [Ajoute ici 1 ou 2 constats personnels : une catégorie qui te surprend, un vendeur qui sort du lot, etc.]

## Méthode
1. Chargement et préparation des données dans Snowflake (SQL).
2. Modélisation des relations entre les tables dans Power BI.
3. Création de mesures en DAX (taux d'annulation, taux d'avis positifs et négatifs, note moyenne).
4. Conception des visuels et des indicateurs du dashboard.

## Outils utilisés
Power BI, DAX, SQL, Snowflake.

## Fichiers du dépôt
- `tableaux de bord des avis.pdf` : export complet du dashboard
- `dashboard.png` : capture d'écran

## Pistes d'amélioration
- Analyser le texte des avis pour identifier les causes des notes basses.
- Comparer les délais de livraison avec la note donnée.
