# 📊 Analyse des Données Clients Olist

## 🧩 Problématique

**Comment segmenter efficacement les clients d’Olist selon leurs comportements d’achat, de localisation et de logistique, afin d’identifier des groupes homogènes pour améliorer la stratégie commerciale ?**

---

## 🔍 Méthodologie

### 1. 📥 Chargement & exploration

* Importation de jeux de données clients, commandes, produits, géolocalisation
* Vérification des valeurs manquantes et des doublons

### 2. 🔄 Prétraitement & fusion

* Jointures entre les bases (`order_id`, `customer_id`)
* Normalisation des variables pour le clustering
* Réduction de dimension via **PCA** (Analyse en Composantes Principales)

### 3. 📚 Clustering non supervisé

Plusieurs méthodes de **segmentation client** ont été testées :

#### 📌 Algorithmes

* **K-Means**
* **DBSCAN**
* **Agglomératif (Hierarchical Clustering)**

#### 🧪 Évaluation comparative :

* 📉 **Elbow Plot** : pour déterminer le nombre optimal de clusters via la distorsion/inertie
* 🧭 **Silhouette Score** : pour mesurer la qualité de séparation entre clusters
* 🎯 **t-SNE** : pour visualiser les clusters en 2D tout en préservant les relations de proximité
* 🔍 **Dendrogrammes** : pour explorer la structure hiérarchique

### 4. 📈 Visualisations

* Cartographie interactive des clusters clients par région
* Graphiques de densité, scatter plots, heatmaps
* Comparaison des clusters selon les délais de livraison, distance, fréquence d’achat, etc.

---

## 🧾 Résultats / Outputs clés

* 📊 **Clusters interprétables** en fonction de la localisation, des habitudes d’achat et des délais
* ✅ **Score de silhouette optimal** obtenu pour le modèle à *n=4* clusters (K-Means)
* 🗺️ **t-SNE** permet une bonne séparation visuelle des groupes
* 📍 Regroupement géographique de certains clusters montrant des disparités régionales

---

## 📌 Conclusion

Le notebook démontre une segmentation client pertinente grâce à une approche rigoureuse de clustering non supervisé. L’usage croisé de **méthodes visuelles (t-SNE, elbow)** et **quantitatives (silhouette)** permet de valider la cohérence des segments. Ces insights sont directement mobilisables pour du ciblage marketing ou de la personnalisation des services logistiques.
