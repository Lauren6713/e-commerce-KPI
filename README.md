# 🛒 Analyse E-commerce – Données Olist (Kaggle)

**Projet Python | Exploration, Visualisation & Analyse Statistique**

## 📌 Description du projet

[cite_start]Ce projet présente une **analyse approfondie du jeu de données public Olist E-commerce Brésilien** (source Kaggle)[cite: 3]. [cite_start]L'étude, menée avec **Python**, explore plus de **100 000 commandes** passées entre 2016 et 2018. Elle met en lumière des **indicateurs clés de performance** et des **insights exploitables** concernant la popularité des produits, la satisfaction client et l'impact des délais de livraison sur les avis[cite: 3].

---

## 🎯 Problématiques Clés

* Quels sont les produits et catégories les plus populaires ?
* Quelles catégories de produits reçoivent les évaluations les plus faibles ?
* Le temps de livraison influence-t-il significativement la satisfaction client ?

---

## 🧠 Approche Analytique

* [cite_start]**Manipulation et Préparation des Données :** Fusion et nettoyage des jeux de données (`pandas`), conversion des champs de date/heure, et traitement des valeurs manquantes[cite: 96, 107, 139, 149, 154].
* [cite_start]**Ingénierie de Caractéristiques :** Création de métriques comme la catégorie de satisfaction des avis et les délais de livraison[cite: 172, 292].
* [cite_start]**Visualisation de Données :** Création de graphiques informatifs avec `matplotlib` et `seaborn`[cite: 10, 200, 232, 260].
* [cite_start]**Analyse Statistique :** Application du test T (`scipy.stats.ttest_ind`) pour évaluer l'impact du temps de livraison sur les scores d'avis[cite: 13, 296, 297].

---

## 🔍 Données & Outils

**Source** : [Kaggle – Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

**Fichiers utilisés** :
* [cite_start]`olist_orders_dataset.csv` [cite: 16]
* [cite_start]`olist_customers_dataset.csv` [cite: 16]
* [cite_start]`olist_order_items_dataset.csv` [cite: 16]
* [cite_start]`olist_order_payments_dataset.csv` [cite: 16]
* [cite_start]`olist_order_reviews_dataset.csv` [cite: 16]
* [cite_start]`olist_products_dataset.csv` [cite: 16]
* [cite_start]`olist_sellers_dataset.csv` [cite: 16]

**Outils** :
* [cite_start]**Environnement :** Python, Jupyter / Google Colab [cite: 6]
* [cite_start]**Librairies :** `pandas` [cite: 8][cite_start], `numpy` [cite: 7][cite_start], `matplotlib` [cite: 10][cite_start], `seaborn` [cite: 11][cite_start], `scipy.stats` [cite: 13]

---

## 📐 Étapes Clés du Projet

### 1. Préparation des Données
* [cite_start]Vérification et suppression des doublons (aucun trouvé)[cite: 86, 92].
* [cite_start]Conversion des colonnes de date/heure au format `datetime` pour tous les DataFrames pertinents[cite: 109, 112].
* [cite_start]Gestion des valeurs manquantes : remplacement des catégories de produits manquantes par 'unknown' et des dimensions/poids par leur moyenne[cite: 139, 149].
* [cite_start]Fusion de tous les jeux de données en un DataFrame `df_all` complet pour l'analyse[cite: 156, 160, 163, 170].

### 2. Ingénierie de Caractéristiques
* [cite_start]Création d'une nouvelle colonne `review_category` ('Excellent', 'Good', 'Average', 'Poor') basée sur le score d'avis[cite: 174, 184].
* [cite_start]Calcul du `delivery_time` en jours (date de livraison client - date d'achat)[cite: 292].

---

## 📊 Résultats et Insights

### 🔝 Catégories de Produits les Plus Vendues
* [cite_start]Les catégories `cama_mesa_banho` (lit, bain, table), `beleza_saude` (beauté, santé), et `esporte_lazer` (sport, loisirs) sont en tête des ventes[cite: 213, 214, 215].

### ⚠️ Catégories de Produits les Moins Bien Notées
* [cite_start]Les catégories `seguros_e_servicos`, `pc_gamer`, et `fraldas_higiene` (couches, hygiène) affichent les scores d'avis moyens les plus bas[cite: 268, 269, 270].

### ⏱ Impact de la Livraison sur la Satisfaction Client
* [cite_start]Les livraisons rapides (inférieures ou égales au temps de livraison médian) obtiennent des scores d'avis clients significativement plus élevés que les livraisons lentes[cite: 300, 301].
* [cite_start]Un **test T** a confirmé que cette différence est **statistiquement significative**, soulignant l'importance de l'efficacité logistique pour la satisfaction client[cite: 13].

---

## 📉 Visualisations Clés

* [cite_start]**Top 10 des catégories de produits les plus vendues**[cite: 201, 223].
* [cite_start]**Répartition des catégories d'avis** (Excellent, Poor, Good, Average)[cite: 233, 243].
* [cite_start]**Top 10 des pires catégories de produits par score d'avis moyen**[cite: 263, 279].
* [cite_start]**Score d'avis moyen pour les livraisons rapides vs. lentes**[cite: 313, 321].

---

## ⚠️ Limites du Jeu de Données

* Données spécifiques au marché brésilien et à la période 2016-2018.
* [cite_start]Certaines données produits (longueur du nom, description, nombre de photos) comportent des valeurs manquantes[cite: 151].
* [cite_start]Les commentaires de revue (titre et message) présentent un nombre significatif de valeurs manquantes[cite: 128].

## 📬 Contact

📧 [lauren.garcia0204@gmail.com](mailto:lauren.garcia0204@gmail.com)

> *Utilisons les données pour améliorer l'expérience e-commerce.*
>
> # 🛒 E-commerce Analysis – Olist Dataset (Kaggle)

**Python Project | Exploration, Visualization & Statistical Analysis**

## 📌 Project Overview

[cite_start]This project presents an **in-depth analysis of the Olist Brazilian E-commerce Public Dataset** (Kaggle source)[cite: 3]. [cite_start]Conducted using **Python**, the study explores over **100,000 orders** placed between 2016 and 2018. It uncovers **key performance indicators** and **actionable insights** regarding product popularity, customer satisfaction, and the impact of delivery times on reviews[cite: 3].

---

## 🎯 Key Questions

* What are the most popular products and categories?
* Which product categories receive the lowest customer ratings?
* Does delivery speed significantly impact customer satisfaction?

---

## 🧠 Analytical Approach

* [cite_start]**Data Manipulation and Preparation:** Merging and cleaning datasets (`pandas`), converting date/time fields, and handling missing values[cite: 96, 107, 139, 149, 154].
* [cite_start]**Feature Engineering:** Creating metrics such as review satisfaction categories and delivery times[cite: 172, 292].
* [cite_start]**Data Visualization:** Generating insightful charts using `matplotlib` and `seaborn`[cite: 10, 200, 232, 260].
* [cite_start]**Statistical Analysis:** Applying T-tests (`scipy.stats.ttest_ind`) to assess the impact of delivery time on review scores[cite: 13, 296, 297].

---

## 🔍 Data & Tools

**Source**: [Kaggle – Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

**Files used**:
* [cite_start]`olist_orders_dataset.csv` [cite: 16]
* [cite_start]`olist_customers_dataset.csv` [cite: 16]
* [cite_start]`olist_order_items_dataset.csv` [cite: 16]
* [cite_start]`olist_order_payments_dataset.csv` [cite: 16]
* [cite_start]`olist_order_reviews_dataset.csv` [cite: 16]
* [cite_start]`olist_products_dataset.csv` [cite: 16]
* [cite_start]`olist_sellers_dataset.csv` [cite: 16]

**Tools**:
* [cite_start]**Environment:** Python, Jupyter / Google Colab [cite: 6]
* [cite_start]**Libraries:** `pandas` [cite: 8][cite_start], `numpy` [cite: 7][cite_start], `matplotlib` [cite: 10][cite_start], `seaborn` [cite: 11][cite_start], `scipy.stats` [cite: 13]

---

## 📐 Key Project Steps

### 1. Data Preparation
* [cite_start]Checked for and confirmed no duplicate rows across datasets[cite: 86, 92].
* [cite_start]Converted relevant date/timestamp columns to `datetime` format in all DataFrames[cite: 109, 112].
* [cite_start]Handled missing values by replacing unknown product categories with 'unknown' and product dimensions/weights with their respective averages[cite: 139, 149].
* [cite_start]Merged all individual datasets into a comprehensive `df_all` DataFrame for unified analysis[cite: 156, 160, 163, 170].

### 2. Feature Engineering
* [cite_start]Created a new `review_category` column ('Excellent', 'Good', 'Average', 'Poor') based on the `review_score`[cite: 174, 184].
* [cite_start]Calculated `delivery_time` in days (customer delivery date - purchase timestamp)[cite: 292].

---

## 📊 Key Findings and Insights

### 🔝 Top Selling Product Categories
* [cite_start]Categories such as `cama_mesa_banho` (bed, bath, table), `beleza_saude` (health, beauty), and `esporte_lazer` (sport, leisure) are among the highest-selling[cite: 213, 214, 215].

### ⚠️ Worst Reviewed Product Categories
* [cite_start]Categories like `seguros_e_servicos` (insurance & services), `pc_gamer`, and `fraldas_higiene` (diapers, hygiene) received the lowest average review scores[cite: 268, 269, 270].

### ⏱ Delivery Impact on Customer Satisfaction
* [cite_start]Faster deliveries (at or below the median delivery time) resulted in significantly higher customer review scores compared to slower deliveries[cite: 300, 301].
* [cite_start]A **T-test** confirmed this difference to be **statistically significant**, highlighting the critical role of logistics efficiency in customer satisfaction[cite: 13].

---

## 📉 Key Visualizations

* [cite_start]**Top 10 Most Sold Product Categories**[cite: 201, 223].
* [cite_start]**Distribution of Review Categories** (Excellent, Poor, Good, Average)[cite: 233, 243].
* [cite_start]**Top 10 Worst Product Categories by Average Review Score**[cite: 263, 279].
* [cite_start]**Average Review Score for Fast vs. Slow Deliveries**[cite: 313, 321].

---

## ⚠️ Dataset Limitations

* Data is specific to the Brazilian market and covers only the 2016–2018 period.
* [cite_start]Some product data (name length, description length, photo quantity) contain missing values[cite: 151].
* [cite_start]Review comments (title and message) have a significant number of missing entries[cite: 128].

## 📬 Contact

📧 [lauren.garcia0204@gmail.com](mailto:lauren.garcia0204@gmail.com)

> *Let’s use data to improve the e-commerce experience.*
