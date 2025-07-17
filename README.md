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

## 🌳 Current Project Tree (with Comments)

```text
Ai-Driven-Healthcare-Webapp/
│
├── app.py                # Streamlit web app entry point
├── disease_pred.py       # Core logic for disease prediction (chat/CLI)
├── model.py              # DiseasePredictor class and ML logic
├── nlp_processor.py      # NLP utilities for symptom extraction
├── symptoms.py           # Loads available symptoms from training data
├── prescriptions.py      # Maps diseases to prescription recommendations
├── train_models.py       # Script to train ML models and save .pkl files
├── evaluate_model.py     # Script to evaluate model performance
│
├── requirements.txt      # Python dependencies for pip
├── pyproject.toml        # Modern Python project config (optional)
├── README.md             # Project documentation
├── LICENSE               # MIT License
├── .gitignore            # Git ignore rules
│
├── generated-icon.png    # App icon for Streamlit UI
├── disease_pred.ipynb    # Jupyter notebook for demo/experiments
│
├── Testing.csv           # Test dataset
├── Training.csv          # Training dataset
│
├── rf_model.pkl          # Trained Random Forest model
├── svm_model.pkl         # Trained SVM model
├── nb_model.pkl          # Trained Naive Bayes model
│
├── verification.py       # (Optional) Model verification utility
├── tempCodeRunnerFile.py # (Temp) VSCode/IDE runner file (can ignore)
│
├── Optimised/            # (Optional) Folder for optimized scripts/models
├── attached_assets/      # (Optional) Extra assets (not core to app)
├── .ipynb_checkpoints/   # Jupyter notebook checkpoints (auto-generated)
├── __pycache__/          # Python bytecode cache (auto-generated)
├── venv/                 # Local Python virtual environment (should be gitignored)
└── uv.lock, replit.nix   # (Optional) Environment/config files for uv/replit
```

---

## 🗂️ Recommended Scalable Structure

For larger teams or future expansion, consider this organization:

```text
Ai-Driven-Healthcare-Webapp/
│
├── src/                        # All source code
│   ├── __init__.py
│   ├── app.py                  # Streamlit entry point
│   ├── disease_pred.py         # Core logic
│   ├── model.py                # ML models
│   ├── nlp_processor.py        # NLP utilities
│   ├── symptoms.py             # Symptom loader
│   ├── prescriptions.py        # Prescription logic
│
├── data/                       # Datasets
│   ├── Training.csv
│   ├── Testing.csv
│
├── models/                     # Trained model binaries
│   ├── rf_model.pkl
│   ├── svm_model.pkl
│   ├── nb_model.pkl
│
├── notebooks/                  # Jupyter notebooks
│   └── disease_pred.ipynb
│
├── assets/                     # Images, icons, etc.
│   └── generated-icon.png
│
├── scripts/                    # Utility scripts (training, evaluation)
│   ├── train_models.py
│   ├── evaluate_model.py
│   └── verification.py
│
├── requirements.txt
├── pyproject.toml
├── README.md
├── LICENSE
├── .gitignore
└── ... (other config files)
```

---

### Benefits of This Structure
- **Separation of concerns:** Code, data, models, and assets are clearly separated.
- **Easier collaboration:** Team members can work on different parts without conflicts.
- **Scalability:** Easy to add new features, models, or datasets.
- **Cleaner root directory:** Only essential project files and configs at the top level.

---

**You can migrate gradually**—start by creating the folders, then move files and update import paths as needed.

Let me know if you want a migration plan or help with updating import statements for this structure!

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
