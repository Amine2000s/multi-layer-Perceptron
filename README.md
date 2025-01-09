# Modèle de classification avec MLP
lien de rapport : https://drive.google.com/file/d/1_e13_MkH1x34IqPzhe0Qoboyrcw1ByJ0/view?usp=sharing

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

# **Classification Model with MLP**  
Report link: [Google Drive Report](https://drive.google.com/file/d/1_e13_MkH1x34IqPzhe0Qoboyrcw1ByJ0/view?usp=sharing)

## Description  
This project consists of developing and testing a multi-layer perceptron (MLP) model to perform binary classification using the modified "bank.csv" dataset.  
The model uses different architectures and parameters to optimize its performance.

### Key Points:  
- Use of hidden layers with activation functions such as ReLU and Tanh.
- Hyperparameter tuning: learning rate, batch size, and epochs.
- Evaluation based on accuracy and loss ("binary_crossentropy").

### Prerequisites  
- **Python**: Version 3.7 or higher  
- **Environment**: Jupyter Notebook  
- **Required Libraries**:  
  - TensorFlow  
  - NumPy  
  - Pandas  
  - Matplotlib  
  - scikit-learn (optional)

## Experiments  
### Experiment 1: Basic MLP  
- Architecture: One input layer with ReLU activation and one output layer with Sigmoid activation.
- Parameters:
  - Loss function: binary_crossentropy  
  - Metric: accuracy  
  - Epochs: 50  
  - Batch size: 32  
  - Learning rate: 0.001  
- **Results**: The performance is decent, but there is room for improvement.

### Experiment 2: Deeper MLP  
- Architecture: One input layer with ReLU activation, two hidden layers (ReLU), and one output layer with Sigmoid activation.
- Parameters:
  - Loss function: binary_crossentropy  
  - Metric: accuracy  
  - Epochs: 50 (increased to 100)  
  - Learning rate: 0.001 (increased to 0.008)  
  - Batch size: 32 (increased to 64)  
- Modifications:
  - Added a Tanh layer (16 neurons).
  - Added additional ReLU layers with 32 and 16 neurons.  
- **Results**: Marginal improvements, but further adjustments are needed.

### Experiment 3: MLP with Tanh Activation  
- Architecture: One input layer and one hidden layer with Tanh activation (16 neurons), and one output layer with Sigmoid activation.
- Parameters:
  - Loss function: binary_crossentropy  
  - Metric: accuracy  
  - Epochs: 50  
  - Batch size: 64  
  - Learning rate: 0.001  
- Modifications:
  - Added two ReLU layers (16 neurons each).  
- **Results**: Adjustments did not significantly improve performance.

## Data  
- **Used data**: `bank.csv`, modified to include:
  - Removal of unnecessary columns like `contact` and `default`.
  - Encoding categorical columns such as `job` and `marital status`.
