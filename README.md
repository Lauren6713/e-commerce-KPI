# 🛒 Analyse E-commerce – Données Olist (Kaggle)

**Projet Python | Exploration, Visualisation & Analyse Statistique**

## 📌 Description du projet

Ce projet présente une **analyse approfondie du jeu de données public Olist E-commerce Brésilien** (source Kaggle). L'étude, menée avec **Python**, explore plus de **100 000 commandes** passées entre 2016 et 2018. Elle met en lumière des **indicateurs clés de performance** et des **insights exploitables** concernant la popularité des produits, la satisfaction client et l'impact des délais de livraison sur les avis.

---

## 🎯 Problématiques Clés

* Quels sont les produits et catégories les plus populaires ?
* Quelles catégories de produits reçoivent les évaluations les plus faibles ?
* Le temps de livraison influence-t-il significativement la satisfaction client ?

---

## 🧠 Approche Analytique

* **Manipulation et Préparation des Données :** Fusion et nettoyage des jeux de données (`pandas`), conversion des champs de date/heure, et traitement des valeurs manquantes.
* **Caractéristiques :** Création de métriques comme la catégorie de satisfaction des avis et les délais de livraison.
* **Visualisation de Données :** Création de graphiques informatifs avec `matplotlib` et `seaborn`.
* **Analyse Statistique :** Application du test T (`scipy.stats.ttest_ind`) pour évaluer l'impact du temps de livraison sur les scores d'avis.

---

## 🔍 Données & Outils

**Source** : [Kaggle – Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

**Fichiers utilisés**:
* `olist_orders_dataset.csv`
* `olist_customers_dataset.csv`
* `olist_order_items_dataset.csv`
* `olist_order_payments_dataset.csv`
* `olist_order_reviews_dataset.csv`
* `olist_products_dataset.csv`
* `olist_sellers_dataset.csv`

**Outils**:
* **Environnement :** Python, Jupyter / Google Colab
* **Librairies :** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy.stats`

---

## 📐 Étapes Clés du Projet

### 1. Préparation des Données
* Vérification et suppression des doublons (aucun trouvé).
* Conversion des colonnes de date/heure au format `datetime` pour tous les DataFrames pertinents.
* Gestion des valeurs manquantes : remplacement des catégories de produits manquantes par 'unknown' et des dimensions/poids par leur moyenne.
* Fusion de tous les jeux de données en un DataFrame `df_all` complet pour l'analyse.

### 2. Ingénierie de Caractéristiques
* Création d'une nouvelle colonne `review_category` ('Excellent', 'Good', 'Average', 'Poor') basée sur le score d'avis.
* Calcul du `delivery_time` en jours (date de livraison client - date d'achat).

---

## 📊 Résultats et Insights

### 🔝 Catégories de Produits les Plus Vendues
* Les catégories `cama_mesa_banho` (lit, bain, table), `beleza_saude` (beauté, santé), et `esporte_lazer` (sport, loisirs) sont en tête des ventes.

### ⚠️ Catégories de Produits les Moins Bien Notées
* Les catégories `seguros_e_servicos` (insurance & services), `pc_gamer`, et `fraldas_higiene` (couches, hygiène) affichent les scores d'avis moyens les plus bas.

### ⏱ Impact de la Livraison sur la Satisfaction Client
* Les livraisons rapides (inférieures ou égales au temps de livraison médian) obtiennent des scores d'avis clients significativement plus élevés que les livraisons lentes.
* Un **test T** a confirmé que cette différence est **statistiquement significative**, soulignant l'importance de l'efficacité logistique pour la satisfaction client.

---

## 📉 Visualisations Clés

* **Top 10 des catégories de produits les plus vendues.**
* **Répartition des catégories d'avis** (Excellent, Poor, Good, Average).
* **Top 10 des pires catégories de produits par score d'avis moyen.**
* **Score d'avis moyen pour les livraisons rapides vs. lentes.**

---

## ⚠️ Limites du Jeu de Données

* Données spécifiques au marché brésilien et à la période 2016-2018.
* Certaines données produits (longueur du nom, description, nombre de photos) comportent des valeurs manquantes.
* Les commentaires de revue (titre et message) présentent un nombre significatif de valeurs manquantes.

## 📬 Contact

📧 [lauren.garcia0204@gmail.com](mailto:lauren.garcia0204@gmail.com)

> *Utilisons les données pour améliorer l'expérience e-commerce.*

---
---

# 🛒 E-commerce Analysis – Olist Dataset (Kaggle)

**Python Project | Exploration, Visualization & Statistical Analysis**

## 📌 Project Overview

This project presents an **in-depth analysis of the Olist Brazilian E-commerce Public Dataset** (Kaggle source). Conducted using **Python**, the study explores over **100,000 orders** placed between 2016 and 2018. It uncovers **key performance indicators** and **actionable insights** regarding product popularity, customer satisfaction, and the impact of delivery times on reviews.

---

## 🎯 Key Questions

* What are the most popular products and categories?
* Which product categories receive the lowest customer ratings?
* Does delivery speed significantly impact customer satisfaction?

---

## 🧠 Analytical Approach

* **Data Manipulation and Preparation:** Merging and cleaning datasets (`pandas`), converting date/time fields, and handling missing values.
* **Feature Engineering:** Creating metrics such as review satisfaction categories and delivery times.
* **Data Visualization:** Generating insightful charts using `matplotlib` and `seaborn`.
* **Statistical Analysis:** Applying T-tests (`scipy.stats.ttest_ind`) to assess the impact of delivery time on review scores.

---

## 🔍 Data & Tools

**Source**: [Kaggle – Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

**Files used**:
* `olist_orders_dataset.csv`
* `olist_customers_dataset.csv`
* `olist_order_items_dataset.csv`
* `olist_order_payments_dataset.csv`
* `olist_order_reviews_dataset.csv`
* `olist_products_dataset.csv`
* `olist_sellers_dataset.csv`

**Tools**:
* **Environment:** Python, Jupyter / Google Colab
* **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy.stats`

---

## 📐 Key Project Steps

### 1. Data Preparation
* Checked for and confirmed no duplicate rows across datasets.
* Converted relevant date/timestamp columns to `datetime` format in all DataFrames.
* Handled missing values by replacing unknown product categories with 'unknown' and product dimensions/weights with their respective averages.
* Merged all individual datasets into a comprehensive `df_all` DataFrame for unified analysis.

### 2. Feature Engineering
* Created a new `review_category` column ('Excellent', 'Good', 'Average', 'Poor') based on the `review_score`.
* Calculated `delivery_time` in days (customer delivery date - purchase timestamp).

---

## 📊 Key Findings and Insights

### 🔝 Top Selling Product Categories
* Categories such as `cama_mesa_banho` (bed, bath, table), `beleza_saude` (health, beauty), and `esporte_lazer` (sport, leisure) are among the highest-selling.

### ⚠️ Worst Reviewed Product Categories
* Categories like `seguros_e_servicos` (insurance & services), `pc_gamer`, and `fraldas_higiene` (diapers, hygiene) received the lowest average review scores.

### ⏱ Delivery Impact on Customer Satisfaction
* Faster deliveries (at or below the median delivery time) resulted in significantly higher customer review scores compared to slower deliveries.
* A **T-test** confirmed this difference to be **statistically significant**, highlighting the critical role of logistics efficiency in customer satisfaction.

---

## 📉 Key Visualizations

* **Top 10 Most Sold Product Categories.**
* **Distribution of Review Categories** (Excellent, Poor, Good, Average).
* **Top 10 Worst Product Categories by Average Review Score.**
* **Average Review Score for Fast vs. Slow Deliveries.**

---

## ⚠️ Dataset Limitations

* Data is specific to the Brazilian market and covers only the 2016–2018 period.
* Some product data (name length, description length, photo quantity) contain missing values.
* Review comments (title and message) have a significant number of missing entries.

## 📬 Contact

📧 [lauren.garcia0204@gmail.com](mailto:lauren.garcia0204@gmail.com)

> *Let’s use data to improve the e-commerce experience.*
