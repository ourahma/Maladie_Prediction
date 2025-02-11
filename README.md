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

```python
import joblib
import pandas as pd

# Charger le modèle
model = joblib.load("model_maladies.pkl")

# Exemple de patient avec symptômes
patient = pd.DataFrame([{ "Âge": 30, "Sexe": 1, "fièvre": 1, "toux": 1, "fatigue": 1, "douleur musculaire": 0, "éruption cutanée": 0, "difficulté respiratoire": 0, "conjonctivite": 0 }])

# Prédire la maladie
prediction = model.predict(patient)
print("Maladie prédite:", prediction[0])
```
## Auteur
Maroua Ourahma  
- Email : marouaourahma@gmail.com 
- LinkedIn : [linkedin.com/in/ourahma](www.linkedin.com/in/maroua-ourahma-293426235)  

