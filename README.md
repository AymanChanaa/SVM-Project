# Classification avec SVM : Crocodiles vs Alligators

Ce projet implémente un modèle de **classification par vecteur de support** (Support Vector Machine, SVM) avec un noyau linéaire pour séparer deux classes de données bidimensionnelles. Les données représentent deux classes : **Crocodiles** et **Alligators**, créées à l’aide de la fonction `make_blobs` de scikit-learn.

## Objectif

L’objectif est de démontrer l’utilisation d’un modèle SVM pour une classification binaire avec des données synthétiques, en visualisant la séparation linéaire générée par le SVM pour distinguer les deux classes.

## Dataset

Les données sont générées avec la fonction `make_blobs` de scikit-learn, qui permet de créer des ensembles de données bidimensionnels pour des tâches de classification supervisée. Les paramètres du jeu de données peuvent être ajustés pour modifier la distribution des points :

- **Nombre de classes** : 2 (Crocodiles et Alligators)
- **Dimensions** : 2 (pour une visualisation facile)
- **Points par classe** : Variable, défini par le paramètre `n_samples`

Exemple de génération de données :
```python
from sklearn.datasets import make_blobs
X, y = make_blobs(n_samples=100, centers=2, random_state=42)
```

## Prérequis

Python 3.11
Jupyter Notebook (facultatif pour une exécution pas-à-pas)

## Bibliothèques :
scikit-learn
matplotlib
numpy
Installation des dépendances

## Pour installer les bibliothèques nécessaires, exécutez la commande suivante :

```bash
pip install scikit-learn matplotlib numpy
```

## Structure du Projet

svm_classification.ipynb : Notebook contenant le code pour générer les données, entraîner le modèle SVM, et visualiser les résultats.
Étapes du Notebook

## Génération des données :

Utilisation de make_blobs pour créer des points représentant les classes Crocodiles et Alligators dans un espace bidimensionnel.

## Division des données :

Division des données en ensembles d'entraînement et de test pour évaluer la performance du modèle.

## Entraînement du modèle SVM :

Création et entraînement d'un classificateur SVM avec un noyau linéaire à l’aide de SVC(kernel="linear") de scikit-learn.

## Évaluation et visualisation :

Affichage de la frontière de décision créée par le SVM.

Visualisation des points de données en fonction de leurs classes et des marges de séparation du modèle.

## Utilisation :

Clonez ce dépôt et ouvrez le fichier svm_classification.ipynb dans Jupyter Notebook.

Exécutez chaque cellule dans l’ordre pour générer les données, entraîner le modèle, et visualiser la séparation.

## Exemple de Résultat :
La sortie inclut une visualisation des données où les classes Crocodiles et Alligators sont séparées par une frontière de décision linéaire. Le SVM avec noyau linéaire parvient à tracer une ligne de séparation optimale entre les deux classes, tout en maximisant la marge entre elles.

## Conclusion :

Ce projet démontre comment un SVM avec noyau linéaire peut être utilisé pour classifier des données bidimensionnelles de manière efficace. Cette approche peut être étendue à des jeux de données réels avec des caractéristiques plus complexes et plusieurs classes.
