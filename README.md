# 🚢 Titanic - Prédiction de Survie avec Machine Learning

Ce projet utilise le jeu de données classique du **Titanic** (recueilli via OpenML) pour construire un modèle prédictif capable de déterminer la survie d'un passager selon plusieurs caractéristiques (âge, tarif, classe, genre et port d'embarquement).

## 📌 Points clés du projet
* **Exploration & Nettoyage :** Audit des valeurs manquantes et visualisation des distributions avec `seaborn` et `matplotlib`.
* **Pipeline de prétraitement (`ColumnTransformer`) :**
  * *Variables numériques (`age`, `fare`) :* Imputation par la médiane + Normalisation (`StandardScaler`).
  * *Variables catégorielles (`embarked`, `sex`, `pclass`) :* Imputation par la valeur la plus fréquente + Encodage (`OneHotEncoder`).
* **Modélisation :** Entraînement d'un classifieur de **Régression Logistique** (`LogisticRegression`).
* **Évaluation :** Analyse des performances via la matrice de confusion et le rapport de classification (Precision, Recall, F1-Score).

## 🛠️ Technologies & Bibliothèques
* **Python 3**
* **pandas** & **scikit-learn**
* **matplotlib** & **seaborn**
