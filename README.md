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

## 🌳 Project Structure

```text
Ai-Driven-Healthcare-Webapp/
│
├── .gitignore            # Git ignore rules
├── LICENSE               # MIT License
├── pyproject.toml        # Python project config (optional)
├── README.md             # Project documentation
├── requirements.txt      # Python dependencies for pip
│
├── assets/               # Images, icons, and static assets
│   └── generated-icon.png
│
├── data/                 # Datasets
│   ├── Testing.csv
│   └── Training.csv
│
├── models/               # Trained model binaries
│   ├── nb_model.pkl
│   ├── rf_model.pkl
│   └── svm_model.pkl
│
├── notebooks/            # Jupyter notebooks for demo/experiments
│   └── disease_pred.ipynb
│
├── scripts/              # Utility scripts (training, evaluation)
│   ├── evaluate_model.py
│   └── train_models.py
│
└── src/                  # All source code
    ├── app.py                # Streamlit web app entry point
    ├── disease_pred.py       # Core logic for disease prediction (chat/CLI)
    ├── model.py              # DiseasePredictor class and ML logic
    ├── nlp_processor.py      # NLP utilities for symptom extraction
    ├── prescriptions.py      # Maps diseases to prescription recommendations
    └── symptoms.py           # Loads available symptoms from training data
```

---

## ⚙️ Setup

1. **Clone the repository**
   ```bash
   git clone <repo-url>
   cd Ai-Driven-Healthcare-Webapp
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
