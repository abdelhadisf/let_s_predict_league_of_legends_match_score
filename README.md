# League of Legends Match Outcome Prediction  
**Machine Learning & Data Mining Project**

## 📘 Introduction  
Ce projet explore l'application de techniques de Machine Learning sur un dataset de matchs de *League of Legends* afin de prédire l'issue des parties et d'analyser les schémas stratégiques.  
Objectifs principaux :
- Prétraitement des données brutes pour améliorer la qualité.
- Application d’algorithmes supervisés et non supervisés.
- Évaluation comparative des performances des modèles.

## 📊 Dataset  
- **Source** : Kaggle (games.csv)  
- **Taille** : 10 000 matchs  
- **Caractéristiques** : 15 variables (first blood, first tower, first baron, kills, dragons, etc.)  
- **Cible** : Équipe gagnante (Team 1 ou Team 2)  
- **Distribution** : Équilibrée  

### 🔧 Prétraitement :
- Suppression des valeurs aberrantes
- Élimination des données manquantes
- Normalisation des variables numériques
- Sélection des caractéristiques pertinentes

## 🤖 Algorithmes Utilisés

### 🟩 Supervised Learning

#### 1. Decision Tree
- **Critère** : Gini Impurity  
- **Points forts** : Bonne précision, interprétable  
- **Faiblesses** : Sensible à l’overfitting  

#### 2. k-Nearest Neighbors (k-NN)
- **Distance** : Euclidienne  
- **Optimisation de k** : Cross-validation  
- **Points forts** : Captation des patterns locaux  
- **Faiblesses** : Coûteux à la prédiction  

#### 3. Naive Bayes
- **Type** : Gaussian  
- **Points forts** : Rapide, efficace sur données indépendantes  
- **Faiblesses** : Hypothèse d’indépendance limitée  

### 🟦 Unsupervised Learning

#### K-Means Clustering
- **Détermination de k** : Méthode du coude  
- **Évaluation** : Silhouette Score  
- **Utilité** : Analyse exploratoire, détection de profils de match  

## 📈 Comparaison des Méthodes

| Critère              | Decision Tree | k-NN     | Naive Bayes | K-Means        |
|----------------------|---------------|----------|-------------|----------------|
| Précision            | Élevée        | Bonne    | Moyenne     | Non applicable |
| Interprétabilité     | Excellente    | Faible   | Moyenne     | Faible         |
| Efficacité           | Bonne         | Faible   | Excellente  | Moyenne        |
| Adaptation au dataset| Très bonne    | Bonne    | Moyenne     | Exploratoire   |

✅ **Recommandation principale** :  
Utiliser les arbres de décision pour la prédiction de résultats grâce à leur précision et lisibilité.

## 🧩 Conclusion  
Le projet a démontré l’efficacité des modèles de Machine Learning dans le contexte des e-sports.  
- **Arbre de décision** : Meilleur pour la prédiction  
- **K-Means** : Intéressant pour l’analyse stratégique  
- **k-NN & Naive Bayes** : Méthodes complémentaires

### 🔮 Pistes futures :
- Ajouter des données sur les performances individuelles
- Explorer des modèles avancés (Ensembles, Deep Learning)
