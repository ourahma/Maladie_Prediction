# Modèle de Classification des Maladies

Ce projet implémente un modèle de classification pour prédire une maladie (Grippe, COVID-19, Rougeole) en fonction des symptômes d'un patient. Il utilise un **Random Forest Classifier** entraîné sur un dataset de 1000 entrées.

## Contenu du projet
- `dataset_maladies.csv` : Dataset contenant les symptômes et la maladie associée.
- `disease_classification.ipynb` : Script d'entraînement du modèle.
- `model_maladies.pkl` : Modèle entraîné sauvegardé.
- `README.md` : Ce fichier expliquant le projet.

## Installation et Exécution
1. **Cloner le projet**
   ```bash
   git clone https://github.com/ourahma/Maladie_Prediction.git
   cd Maladie_Prediction
   ```


2. **Exécuter l'entraînement du modèle**
   ```bash
   python disease_classification.ipynb
   ```

## Prédiction avec le modèle
Après l'entraînement, vous pouvez charger et utiliser le modèle pour prédire une maladie en fonction des symptômes :


## La performance de modele

- **La précision : 89%**
```python
Accuracy: 0.89
              precision    recall  f1-score   support

    COVID-19       0.82      0.92      0.87        63
      Grippe       0.92      0.80      0.85        69
    Rougeole       0.94      0.96      0.95        68

    accuracy                           0.89       200
   macro avg       0.89      0.89      0.89       200
weighted avg       0.89      0.89      0.89       200

```
## Auteur
Maroua Ourahma  
- Email : marouaourahma@gmail.com 
- LinkedIn : [linkedin.com/in/ourahma](www.linkedin.com/in/maroua-ourahma-293426235)  

