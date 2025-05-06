# 📊 Analyse des Données Clients Olist

## 🧩 Problématique

Comment mieux comprendre le comportement des clients d’Olist à travers l’analyse des données transactionnelles, logistiques et géographiques, afin d’identifier les facteurs influençant la satisfaction et la fidélisation ?

---

## 🔍 Méthodologie

Le notebook suit une démarche en plusieurs étapes :

### 1. 📥 Chargement et exploration des données

* Lecture de fichiers CSV (`customers`, `orders`, `geolocation`, etc.)
* Aperçu des dimensions, types et valeurs manquantes

### 2. 🧬 Fusion et nettoyage

* Jointures sur des identifiants (`customer_id`, `order_id`)
* Suppression de doublons et gestion des valeurs nulles

### 3. 🗺️ Analyse géographique

* Nettoyage des données de géolocalisation (cohérence des coordonnées)
* Visualisation de la répartition des clients par État (via `plotly` ou `seaborn`)

### 4. 📦 Analyse des commandes

* Délai entre achat, expédition et livraison
* Écart entre date promise et date réelle

### 5. 📈 Visualisations

* Répartition temporelle des commandes
* Heatmaps géographiques
* Histogrammes de fréquence et délais
* 

## 📌 Résumé

Ce notebook fournit une base analytique solide pour étudier le parcours client chez Olist. L’intégration des différentes sources de données (commandes, localisation, délais) permet une compréhension fine des freins logistiques et des comportements régionaux. 
