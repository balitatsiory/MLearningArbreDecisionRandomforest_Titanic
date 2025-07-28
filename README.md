# MLearningArbreDecisionRandomforest_Titanic

# 🎯 Titanic - Analyse Prédictive de Survie

Ce projet applique des techniques de Machine Learning pour prédire la survie des passagers du Titanic en fonction de leurs caractéristiques (âge, sexe, classe sociale, etc.). Il repose sur le dataset classique de Kaggle ["Titanic: Machine Learning from Disaster"](https://www.kaggle.com/c/titanic).

## 📂 Contenu du projet

- 🔄 Prétraitement des données (imputation, encodage, suppression colonnes inutiles)
- 🔍 Analyse exploratoire (visualisations, corrélations)
- 🧠 Entraînement de modèles :
  - `DecisionTreeClassifier`
  - `RandomForestClassifier`
- 📈 Évaluation des modèles (Accuracy, Précision, Rappel, F1, ROC)
- 🧪 Optimisation avec `GridSearchCV`
- 📊 Interprétation des résultats

---

## 📌 Objectifs

- Comprendre l'impact des variables comme `Sex`, `Pclass`, `Fare`, `Title` sur la survie
- Comparer différents modèles d'apprentissage supervisé
- Mettre en place une pipeline robuste de modélisation

---

## ⚙️ Technologies utilisées

- Python 3
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- Graphviz (pour affichage de l’arbre de décision)

---

## 📊 Aperçu des résultats

| Modèle                     | Accuracy (Test) |
|---------------------------|-----------------|
| DecisionTree (max_depth=4)| ~0.80           |
| RandomForest (optimisé)   | **0.835** ✅     |

- 🥇 Variable la plus discriminante : **Sex**
- 🛠️ Meilleurs hyperparamètres :  
  `max_depth=10`, `min_samples_split=10`, `n_estimators=100`

---

## 🧠 Conclusion

- La **Random Forest** surpasse l’arbre de décision seul.
- Le modèle est stable et généralise bien.
- Certaines variables créées (`Title`, `FamilySize`, etc.) améliorent les performances.

---

## 🚀 À venir / pistes d'amélioration

- Déploiement avec Streamlit ou Flask


