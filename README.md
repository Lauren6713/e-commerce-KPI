# 🛒 Analyse E-commerce – Données Olist (Kaggle)

**Projet Python | Exploration, Visualisation & Analyse Statistique**

## 📌 Description du projet

Ce projet explore les données du e-commerce brésilien issues de la plateforme **Olist** (source Kaggle). L’analyse couvre plus de **100 000 commandes** passées entre 2016 et 2018. Grâce à Python, le projet met en lumière des **indicateurs clés** de performance et des **insights exploitables** à travers la visualisation et la statistique.

---

## 🎯 Problématiques

* Quels sont les produits les plus populaires ?
* Quelles catégories de produits reçoivent les plus mauvaises évaluations ?
* Le temps de livraison influence-t-il la satisfaction client ?

---

## 🧠 Approche analytique

* Fusion et nettoyage des jeux de données (`pandas`)
* Conversion des dates et traitement des valeurs manquantes
* Création de métriques : score moyen, délais de livraison, catégories de satisfaction
* Visualisations avec `matplotlib` et `seaborn`
* Analyse statistique : test T sur les scores de review en fonction du temps de livraison

---

## 🔍 Données & outils

**Source** : [Kaggle – Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

**Fichiers utilisés** :

* `olist_orders_dataset.csv`
* `olist_customers_dataset.csv`
* `olist_order_items_dataset.csv`
* `olist_order_payments_dataset.csv`
* `olist_order_reviews_dataset.csv`
* `olist_products_dataset.csv`
* `olist_sellers_dataset.csv`

**Outils** :

* Python, Jupyter / Google Colab
* `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`

---

## 📐 Étapes clés

### 1. Préparation des données

* Conversion des champs de date
* Remplacement des valeurs manquantes 
* Fusion de tous les jeux de données en un DataFrame complet

### 2. Création de variables

* Score review → catégorie : *Excellent / Good / Average / Poor*
* Temps de livraison = date de réception – date d’achat

---

## 📊 Résultats

### 🔝 Produits les plus vendus

* Les catégories *bed\_bath\_table*, *health\_beauty* sont en tête.

### ⚠️ Produits les moins bien notés

* Catégories avec score moyen < 3 : *fashion\_underwear\_beach*, *auto*.

### ⏱ Livraison vs Satisfaction

* Les livraisons rapides obtiennent des notes plus élevées.
  Test T → résultat **statistiquement significatif**.

---

## 📉 Visualisations

* Histogramme des catégories de review
* Top 10 des catégories par ventes
* Bar chart des pires catégories (score moyen)
* Comparaison Fast vs Slow delivery (review score moyen)

---

## ⚠️ Limites

* Données limitées au Brésil et à 2016–2018
* Données produit peu granulaires
* Reviews parfois incomplètes (commentaires manquants)

## 📬 Contact

📧 [lauren.garcia0204@gmail.com](mailto:lauren.garcia0204@gmail.com)

> *Utilisons les données pour améliorer l'expérience e-commerce.*

---

## 📌 Project Overview

This project explores the **Brazilian e-commerce dataset** from **Olist** (via Kaggle), analyzing over **100,000 orders** from 2016 to 2018. The goal is to extract **key performance indicators** and provide **actionable insights** using Python, data visualization, and statistics.

---

## 🎯 Key Questions

* What are the most sold product categories?
* Which products have the worst customer reviews?
* Does delivery speed impact customer satisfaction?

---

## 🧠 Analytical Approach

* Merge and clean all datasets using `pandas`
* Convert date fields and handle missing values
* Create calculated features: delivery time, review category
* Visualize with `matplotlib` and `seaborn`
* Perform T-test to evaluate the impact of delivery time on review scores

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

* Python, Jupyter / Google Colab
* `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`

---

## 📐 Key Steps

### 1. Data Preparation

* Convert timestamp fields
* Replace missing values (`unknown`, averages)
* Merge all tables into a unified DataFrame

### 2. Feature Engineering

* Review score → Review category: *Excellent / Good / Average / Poor*
* Delivery time = delivered\_date – purchase\_date

---

## 📊 Key Findings

### 🔝 Top Selling Products

* Categories like *bed\_bath\_table* and *health\_beauty* rank highest.

### ⚠️ Worst Reviewed Products

* Categories with average score < 3: *fashion\_underwear\_beach*, *auto*

### ⏱ Delivery vs Satisfaction

* Faster deliveries lead to better review scores.
  T-test result: **statistically significant**

---

## 📉 Visualizations

* Histogram of review categories
* Top 10 product categories by sales
* Bar chart of worst-reviewed categories
* Avg. score comparison: fast vs slow delivery

---

## ⚠️ Limitations

* Dataset limited to Brazil and 2016–2018 period
* Product-level data lacks subcategories
* Incomplete review texts for some entries

## 📬 Contact

📧 [lauren.garcia0204@gmail.com](mailto:lauren.garcia0204@gmail.com)

> *Let’s use data to improve the e-commerce experience.*
