# Parkinson's Disease Detection using Machine Learning

A machine learning web application that predicts whether a person has Parkinson's Disease based on biomedical voice measurements.

## Live Demo
[Click here to try the app](https://parkinsons-disease-detection-new.streamlit.app)

## About the Project
Parkinson's disease is a progressive nervous system disorder that affects movement. This project uses a Machine Learning model trained on biomedical voice measurements to predict the likelihood of Parkinson's disease in a person.

## Dataset
- Dataset used: [Parkinson's Disease Dataset](https://archive.ics.uci.edu/ml/datasets/parkinsons) from UCI Machine Learning Repository
- The dataset contains biomedical voice measurements from 197 people, 147 of whom have Parkinson's disease
- Features include various vocal frequency and noise measurements

## Features Used
| Feature | Description |
|--------|-------------|
| MDVP:Fo(Hz) | Average vocal fundamental frequency |
| MDVP:Fhi(Hz) | Maximum vocal fundamental frequency |
| MDVP:Flo(Hz) | Minimum vocal fundamental frequency |
| MDVP:Jitter(%) | Variation in fundamental frequency |
| MDVP:Shimmer | Variation in amplitude |
| NHR, HNR | Noise to harmonic ratio measures |
| RPDE, DFA | Nonlinear dynamical complexity measures |
| spread1, spread2, D2, PPE | Nonlinear measures of fundamental frequency variation |

## ML Model
- Algorithm: Support Vector Machine (SVM)
- Library: scikit-learn
- Accuracy: 0.8717948717948718

## Tech Stack
- Python
- Streamlit
- Scikit-learn
- NumPy
- Pickle

## How to Run Locally
1. Clone the repository
```bash
   git clone https://github.com/<trazhboi>/Parkinsons-Disease-Detection.git
```
2. Install dependencies
```bash
   pip install -r requirements.txt
```
3. Run the app
```bash
   streamlit run ParkinsonsWebApp.py
```

## Project Structure
```
Parkinsons-Disease-Detection/
├── ParkinsonsWebApp.py       # Main Streamlit app
├── trained_model.sav         # Saved ML model
├── requirements.txt          # Dependencies
└── README.md                 # Project documentation
```

## Screenshot
<img width="1918" height="970" alt="Screenshot 2026-03-22 181244" src="https://github.com/user-attachments/assets/c0739250-78f2-4e78-9590-f8f16b07c721" />

## Acknowledgements
- Dataset: UCI Machine Learning Repository
- [Streamlit](https://streamlit.io) for the web framework
```

---

**requirements.txt** — you should already have this, double check it has:
```
scikit-learn
streamlit
numpy
