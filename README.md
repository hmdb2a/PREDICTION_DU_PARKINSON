# Prédiction de la maladie de Parkinson par apprentissage automatique

Classification de patients atteints ou non de la maladie de Parkinson à partir de mesures de la voix, en comparant plusieurs modèles d'apprentissage supervisé.

Projet du cours d'introduction à l'apprentissage statistique de la Licence Informatique (Université Paris-Saclay), réalisé en binôme.

## Données

Jeu de données [Parkinson (Kaggle)](https://www.kaggle.com/datasets/sagarbapodara/parkinson-csv) : 195 enregistrements, 24 colonnes de mesures vocales (fréquences, variations d'amplitude). La colonne `status` vaut 1 pour une personne malade et 0 sinon.

## Démarche

1. **Exploration** : contrôle des valeurs manquantes, statistiques descriptives, distribution de chaque variable, corrélations (heatmap).
2. **Préparation** : rééquilibrage des classes par sur-échantillonnage (147 malades contre 48 non malades), mise à l'échelle des variables, réduction de dimension par ACP (95 % de variance conservée).
3. **Modélisation** : entraînement et comparaison de régression logistique, arbre de décision, Random Forest, SVC, k plus proches voisins et XGBoost.
4. **Évaluation** : précision, score F1, matrice de confusion et courbes ROC pour chaque modèle.

## Technologies

Python, Jupyter Notebook, pandas, NumPy, scikit-learn, imbalanced-learn, XGBoost, Matplotlib, seaborn

## Lancer le notebook

```bash
pip install pandas numpy scikit-learn imbalanced-learn xgboost matplotlib seaborn lux-api notebook
jupyter notebook BOUNDAOUI_SARAH_BAAROUN_AHMED.ipynb
```

Le fichier `parkinsons.csv` doit se trouver dans le même dossier que le notebook.

## Contenu du dépôt

| Fichier | Contenu |
|---|---|
| `BOUNDAOUI_SARAH_BAAROUN_AHMED.ipynb` | Notebook complet : exploration, préparation, modèles |
| `parkinsons.csv` | Jeu de données |
| `docs/Rapport.pdf` | Rapport du projet |

## Auteurs

Sarah Boundaoui, Ahmed Baaroun
