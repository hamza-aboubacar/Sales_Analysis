# Projet : Analyse des Ventes et Insights Commerciaux
## 📝 Description du Projet
Ce projet a pour objectif de fournir une analyse approfondie des données de ventes afin d'identifier des tendances clés, des performances produits, et des opportunités d'optimisation commerciale. En transformant les données brutes en insights exploitables, ce projet aide les entreprises à prendre des décisions stratégiques pour améliorer leurs revenus, leur rentabilité et l'efficacité de leurs opérations.

Le projet inclut des scripts d'analyse de données en Python et des recommandations pour la création de dashboards interactifs, principalement avec Power BI Desktop.

## 🎯 Problème Métier Addréssé
Dans un environnement commercial dynamique, comprendre les performances des ventes est essentiel. Ce projet répond à des questions fondamentales pour les équipes de vente, de marketing et de direction, telles que :

Quels sont nos produits les plus performants et les moins performants ?

Comment nos ventes évoluent-elles au fil du temps ?

Quelle est la relation entre nos ventes et nos profits ?

Comment optimiser nos stratégies de remise ?

Quels sont les moteurs de vente par région ?

## ✨ Fonctionnalités et Analyses Clés
Ce projet permet de réaliser les analyses suivantes pour obtenir des insights commerciaux précis :

Top/Bottom 5 des Produits :

Identification des 5 meilleurs et des 5 moins bons produits en termes de ventes totales, de profit généré et de quantité vendue.

Tendances des Ventes au Fil du Temps :

Analyse de l'évolution des ventes et des profits sur différentes granularités temporelles : quotidienne, mensuelle, trimestrielle et annuelle.

Relation Ventes & Profit :

Visualisation de la corrélation entre le volume des ventes et la rentabilité, permettant d'identifier si les produits à forte vente sont également les plus profitables.

Comparaison de Périodes :

Capacité à comparer les ventes, les profits et les quantités vendues entre deux périodes définies par l'utilisateur (par exemple, un trimestre par rapport au précédent, ou une année par rapport à l'année précédente).

Remise Moyenne par Catégorie :

Calcul de la remise moyenne offerte pour chaque catégorie de remise (si applicable dans les données), utile pour évaluer l'efficacité des promotions.

Nombre Total de Commandes :

Indicateur clé du volume d'activité commerciale.

Détails des Commandes avec Filtres Visuels :

Affichage des détails de chaque commande (Ventes, Profit, Remise, Ventes Nettes, et autres champs pertinents) avec la possibilité de filtrer dynamiquement par :

Produit

Date

ID Client

Catégories de Promotion

Ventes par Ville :

Analyse de la performance des ventes par différentes villes ou régions géographiques.

## 💻 Technologies et Dépendances
Analyse et Traitement des Données :

Python 3.x

pandas : Pour la manipulation et l'analyse des données.

numpy : Pour les opérations numériques.

(Optionnel) matplotlib, seaborn, plotly : Pour des visualisations initiales en Python.

Base de Données (si applicable) :

SQL : Pour l'extraction et la préparation des données si elles résident dans une base de données relationnelle.

Business Intelligence & Visualisation Interactive :

Power BI Desktop : Pour la création des dashboards interactifs et des rapports. (Alternative : Tableau Desktop)

📁 Structure du Projet
sales_analysis_project/
├── data/                           # Dossier pour les données brutes et traitées
│   └── sales_data.csv              # Exemple de fichier de données de ventes
├── scripts/                        # Dossier pour les scripts Python
│   └── data_preprocessing.py       # Script de nettoyage et préparation des données
│   └── sales_analysis.py           # Script d'analyse Python (calculs, agrégations)
├── dashboards/                     # Dossier pour les fichiers de dashboards BI
│   └── sales_dashboard.pbix        # Exemple de fichier Power BI Desktop
│   └── (sales_dashboard.twbx)      # (Optionnel) Exemple de fichier Tableau Workbook
└── README.md                       # Ce fichier de documentation

## 🚀 Étapes de Réalisation du Projet
Suivez ces étapes pour mettre en place et explorer le projet.

1. **Acquisition et Préparation des Données**
   
Source de Données : Ce projet suppose l'utilisation d'un jeu de données de ventes. Un exemple typique pourrait inclure des colonnes comme OrderID, OrderDate, ProductID, ProductName, Quantity, UnitPrice, Sales, Profit, Discount, CustomerCity, CustomerID, PromotionCategory.

Vous pouvez utiliser un jeu de données public (ex: Superstore Sales sur Kaggle) ou générer des données synthétiques si nécessaire.

Nettoyage et Prétraitement :

Utilisez le script scripts/data_preprocessing.py pour charger vos données, gérer les valeurs manquantes, corriger les types de données (ex: convertir les dates, s'assurer que les chiffres sont numériques) et effectuer toute transformation nécessaire.

Exemple de commande : python scripts/data_preprocessing.py

Output attendu : Un fichier de données nettoyées et prêtes à l'emploi (ex: processed_sales_data.csv) sera sauvegardé dans le dossier data/.


2. **Création de Dashboards Interactifs (Power BI)**
   
Cette étape cruciale transforme les analyses brutes en visualisations interactives pour les utilisateurs finaux, en se concentrant sur Power BI.

Importation des Données :

Ouvrez Power BI Desktop.

Importez le fichier processed_sales_data.csv (et les autres fichiers de résumé générés par sales_analysis.py) comme sources de données.

Construction du Dashboard :

Top/Bottom 5 : Créez des barres ou des tableaux pour les top/bottom 5 produits par ventes, profit, quantité.

Tendances Temporelles : Utilisez des graphiques en ligne pour les ventes et profits quotidiens, mensuels, trimestriels, annuels.

Relation Ventes & Profit : Créez un nuage de points (scatter plot) ou un graphique à bulles (bubble chart) pour visualiser cette relation.

Comparaison de Périodes : Utilisez des paramètres ou des filtres pour permettre à l'utilisateur de sélectionner deux périodes et afficher des graphiques comparatifs (barres, lignes).

Remise Moyenne : Créez un graphique à barres ou un tableau montrant la remise moyenne par catégorie de remise.

Total des Commandes : Affichez ce KPI sous forme de carte ou d'indicateur.

Détails des Commandes : Créez un tableau détaillé des commandes avec des filtres interactifs (produit, date, ID client, promotion).

Ventes par Ville : Utilisez une carte géographique ou un graphique à barres pour visualiser les ventes par ville.

Interactivité :

Ajoutez des filtres globaux (Date Range, Catégorie de Produit, Région, etc.) pour permettre une exploration dynamique des données.

Configurez des actions pour que la sélection d'un élément dans un graphique mette à jour les autres visualisations.

Output attendu : Un fichier de dashboard interactif (ex: .pbix pour Power BI) sera sauvegardé dans le dossier dashboards/.

## Quelques captures d'images

<img width="1284" height="688" alt="Capture d'écran 2025-08-07 120546" src="https://github.com/user-attachments/assets/186fa852-00e9-4be0-885e-e016fc6a4894" />


<img width="1284" height="719" alt="Capture d'écran 2025-08-07 120705" src="https://github.com/user-attachments/assets/3dff5054-590e-46da-bf86-38e9b6e96e7c" />


<img width="1244" height="720" alt="Capture d'écran 2025-08-07 120629" src="https://github.com/user-attachments/assets/17ce3752-833a-44a8-a785-2c4d31a4b3bb" />



## ✍️ Auteur
Aboubacar Halidou Hamza



📄 Licence
Ce projet est sous licence MIT.
