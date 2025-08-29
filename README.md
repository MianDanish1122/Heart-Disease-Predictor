# 🩺 Disease Predictor using Machine Learning

This project predicts diseases based on patient symptoms using **Logistic Regression** and **Random Forest Classifier**.  
The model is trained on a dataset of symptoms and their corresponding diseases.  
It automatically selects the best-performing model and saves it using **Joblib** for future predictions.

---

## 📂 Project Structure

DISEASE_PREDICTOR/
│── data/
│ └── dataset.csv # Dataset (symptoms + disease labels)
│── DISEASE_PREDICTOR.ipynb # Main Jupyter Notebook
│── disease_predictor_model.pkl # Saved ML model (generated after training)
│── requirements.txt # Python dependencies
│── README.md # Project documentation
│── .gitignore



---

## ⚙️ Installation

Clone the repository:
```bash
git clone https://github.com/your-username/DISEASE_PREDICTOR.git
cd DISEASE_PREDICTOR


pip install -r requirements.txt


fever,cough,headache,fatigue,disease
1,0,1,0,Flu
0,1,1,1,Cold


jupyter notebook DISEASE_PREDICTOR.ipynb

import joblib

model = joblib.load("disease_predictor_model.pkl")
sample = [[1, 0, 1, 0, 1]]  # Example patient symptoms
print("Predicted Disease:", model.predict(sample))
