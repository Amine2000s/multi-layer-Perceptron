# Modèle de classification avec MLP

## Description
Ce projet consiste à développer et tester un modèle de perceptron multicouche (MLP) pour effectuer une classification binaire à l'aide du jeu de données modifié "bank.csv".  
Le modèle utilise différentes architectures et paramètres pour optimiser ses performances.  

### Points clés :
- Utilisation de couches cachées avec des fonctions d'activation telles que ReLU et Tanh.
- Ajustement des hyperparamètres : taux d'apprentissage, taille des batches, et époques.
- Évaluation basée sur la précision et la perte ("binary_crossentropy").
### Prérequis
- **Python** : version 3.7 ou supérieure  
- **Environnement** : Jupyter Notebook  
- **Bibliothèques nécessaires** :
  - TensorFlow
  - NumPy
  - Pandas
  - Matplotlib
  - scikit-learn (optionnel)

## Expériences
### Expérience 1 : MLP de base
- Architecture : Une couche d'entrée avec activation ReLU et une couche de sortie avec activation Sigmoïde.
- Paramètres :
  - Fonction de perte : binary_crossentropy  
  - Métrique : précision  
  - Époques : 50  
  - Taille du batch : 32  
  - Taux d'apprentissage : 0.001  
- **Résultats** : Les performances sont correctes, mais il existe un potentiel d'amélioration.

### Expérience 2 : MLP plus profond
- Architecture : Une couche d'entrée avec activation ReLU, deux couches cachées (ReLU), et une couche de sortie avec activation Sigmoïde.
- Paramètres :
  - Fonction de perte : binary_crossentropy  
  - Métrique : précision  
  - Époques : 50 (puis augmenté à 100)  
  - Taux d'apprentissage : 0.001 (puis augmenté à 0.008)  
  - Taille du batch : 32 (puis augmenté à 64)  
- Modifications :
  - Ajout d'une couche Tanh (16 neurones).
  - Ajout de couches ReLU supplémentaires avec 32 et 16 neurones.  
- **Résultats** : Des améliorations marginales, mais nécessitant encore des ajustements.

### Expérience 3 : MLP avec activation Tanh
- Architecture : Une couche d'entrée et une couche cachée avec activation Tanh (16 neurones), et une couche de sortie avec activation Sigmoïde.
- Paramètres :
  - Fonction de perte : binary_crossentropy  
  - Métrique : précision  
  - Époques : 50  
  - Taille du batch : 64  
  - Taux d'apprentissage : 0.001  
- Modifications :
  - Ajout de deux couches ReLU (16 neurones chacune).  
- **Résultats** : Les ajustements n'ont pas significativement amélioré la performance.

## Données
- ** données utilisé** : `bank.csv`, modifié pour inclure :
  - Suppression de colonnes inutiles comme `contact` et `default`.
  - Encodage des colonnes catégorielles comme `job` et `marital status`.

lien de rapport : https://drive.google.com/file/d/1_e13_MkH1x34IqPzhe0Qoboyrcw1ByJ0/view?usp=sharing
