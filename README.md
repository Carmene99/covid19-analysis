# 📊 Analyse Multidimensionnelle de la Pandémie COVID-19

## 📝 Description du Projet
Ce projet présente une analyse interactive réalisée sous **Power BI**, visant à croiser l'évolution des cas de contamination, les campagnes de vaccination et l'impact des politiques gouvernementales à l'échelle mondiale.

## 🗂️ Sources des Données
L'analyse repose sur l'intégration de trois jeux de données distincts et complémentaires :

1.  **Suivi des Cas (Epidémiologie) :** `covid_19_clean_complete.csv`
    * **Source :** [Kaggle](https://www.kaggle.com/imdevskp/corona-virus-report)
    * **Contenu :** Données nettoyées sur les cas confirmés, décès et guérisons.
2.  **Campagnes de Vaccination :** `vaccinations.csv`
    * **Source :** [Our World in Data](https://ourworldindata.org/covid-vaccinations)
    * **Contenu :** État d'avancement des doses administrées par pays.
3.  **Réponses Gouvernementales :** `OxCGRT_latest.csv`
    * **Source :** [Oxford COVID-19 Government Response Tracker](https://github.com/OxCGRT/covid-policy-tracker)
    * **Contenu :** Indicateurs sur la rigueur des mesures (confinements, fermetures d'écoles, etc.).

## 🛠️ Méthodologie (Pipeline Data)
* **ETL (Power Query) :** Nettoyage des données, gestion des valeurs manquantes et normalisation des noms de pays pour permettre la jointure entre les trois fichiers.
* **Modélisation :** Création d'un modèle en étoile reliant les faits (Cas, Vaccins, Mesures) via une table de dimension temporelle et géographique.
* **DAX :** Création de mesures calculées (Taux de létalité, % de population vaccinée, Score de rigueur moyen).

## 📈 Visualisations Clés
* **Dashboard Épidémique :** Évolution temporelle des courbes de contamination.
* **Corrélation Mesures/Cas :** Analyse de l'efficacité des décisions gouvernementales sur la propagation.
* **Impact de la Vaccination :** Comparaison entre la couverture vaccinale et la baisse de la mortalité.

## 🚀 Comment visualiser le rapport
1. Téléchargez le fichier `.pbix` présent dans ce dépôt.
2. Ouvrez-le avec **Power BI Desktop**.
