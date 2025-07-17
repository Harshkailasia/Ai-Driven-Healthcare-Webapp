# 🩺 Disease Prediction System

A machine learning-powered web app for predicting diseases from symptoms, with explainable results and prescription suggestions. Built for rapid prototyping, research, and real-world deployment using Streamlit.

---

## 🚀 Features
- 🤖 Predicts diseases based on user-input symptoms
- 🧠 Uses Random Forest, SVM, and Naive Bayes models (ensemble)
- 📝 NLP preprocessing for robust symptom matching
- 📊 Model evaluation and performance metrics
- 💊 Prescription recommendations for predicted diseases
- 📈 Jupyter notebook for exploration and demo
- 🖼️ Modern, interactive UI with Streamlit

---

## 🏗️ Project Structure

```
T2/
├── app.py                # Streamlit web app entry point
├── disease_pred.py       # Core logic for prediction
├── model.py              # Model classes and utilities
├── nlp_processor.py      # NLP preprocessing
├── symptoms.py           # Symptom list
├── prescriptions.py      # Prescription logic
├── train_models.py       # Model training script
├── evaluate_model.py     # Model evaluation script
├── requirements.txt      # Python dependencies
├── README.md             # Project documentation
├── rf_model.pkl          # Trained Random Forest model
├── svm_model.pkl         # Trained SVM model
├── nb_model.pkl          # Trained Naive Bayes model
├── Training.csv          # Training data
├── Testing.csv           # Test data
├── disease_pred.ipynb    # Jupyter notebook demo
└── ...
```

---

## ⚙️ Setup

1. **Clone the repository**
   ```bash
   git clone <repo-url>
   cd T2
   ```
2. **Create and activate a virtual environment**
   ```bash
   python -m venv venv
   # On Windows:
   venv\Scripts\activate
   # On Mac/Linux:
   source venv/bin/activate
   ```
3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

---

## 🖥️ Usage

### 🌐 Run the Streamlit Web App
```bash
streamlit run app.py
```
- Open the provided local URL in your browser.
- Enter your symptoms in the chat to get predictions and recommendations.

### 🧪 Retrain Models (Optional)
```bash
python train_models.py
```
- This will retrain and overwrite the `.pkl` model files using `Training.csv`.

### 📊 Evaluate Models (Optional)
```bash
python evaluate_model.py
```
- Outputs accuracy and confusion matrix for the current models.

### 📓 Explore in Jupyter Notebook
```bash
jupyter notebook disease_pred.ipynb
```

---

## 🤝 Contributing

Contributions are welcome! Please:
- Fork the repo and create a feature branch
- Add/modify code with clear docstrings and comments
- Write or update tests if needed
- Submit a pull request with a clear description

---

## 📄 License

This project is licensed under the MIT License.
