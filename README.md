# Disease Classification ML Pipeline 🏥

![Python](https://img.shields.io/badge/Python-3.8%2B-blue) 
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.2.2-orange) 
![License](https://img.shields.io/badge/License-MIT-green)

A machine learning system that classifies diseases from clinical symptoms using KNN and Logistic Regression.

## Quick Start ▶️
```bash
git clone https://github.com/yourusername/disease-classifier.git
cd disease-classifier
pip install -r requirements.txt
```

```python
from predictor import DiseasePredictor
model = DiseasePredictor.load('model.pkl')
model.predict([["fever", "cough"]])  # Returns: ['Respiratory Infection']
```

## Key Features ✨
- **Algorithms**: KNN & Logistic Regression
- **Encodings**: TF-IDF & One-Hot
- **Metrics**: Accuracy, Precision, Recall, F1
- **Deployment**: Ready-to-use predictor class

## Data Format 📝
```csv
Risk_Factors,Symptoms,Signs,Disease
"smoking,obesity","cough,fever","high_temp,wheezing",COPD
```

## Results
| Model          | Accuracy | F1-Score |
|----------------|----------|----------|
| KNN            | 0.87     | 0.85     |
| Logistic Reg   | 0.83     | 0.81     |
