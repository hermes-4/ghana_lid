# Language Identification for Ghanaian Languages  

This project focuses on automatic Language Identification (LID) for four under-resourced Ghanaian languages: Akan, Ewe, Ga, and Dagbani.  
The goal is to build and evaluate models that can accurately classify a given text into its language category.  

---

## 📖 Project Overview  
Language Identification has been well-studied for high-resource languages (English, French, Spanish, etc.), but local Ghanaian languages remain underrepresented.  
This project explores how traditional ML models (Logistic Regression, Naive Bayes, SVM) perform when trained on carefully collected and preprocessed corpora of Ghanaian languages.  

---

## 📂 Repository Structure  


```
ghana_lid/
├── data/
│   ├── preprocessing/            # Preprocessing scripts per language
│   │   ├── akan_preprocess.ipynb   # Akan preprocessing
│   │   ├── dagbani_preprocess.ipynb   # Dagbani preprocessing
│   │   ├── ewe_preprocess.ipynb    # Ewe preprocessing
│   │   └── ga_preprocess.ipynb     # Ga preprocessing
│   ├── processed/                # Cleaned & ready-to-use datasets
│   │   ├── dagbani_corpus.json
│   │   ├── ewe_corpus.json
│   │   ├── ga_corpus.json
│   │   └── twi_corpus.json
│   └── README.md                 # Documentation + data source links
├── main_notebook.ipynb           # Full pipeline (EDA → Training → Evaluation)
├── requirements.txt              # Dependencies for reproducibility
└── README.md                     # (this file)

```

---

## ⚙️ Installation & Setup  

Clone the repository:  
```bash
git clone https://github.com/hermes_4/ghana_lid.git
cd ghana_lid
```


Create and activate a virtual environment (recommended):

```bash
python -m venv venv
source venv/bin/activate   # for Linux/Mac
venv\Scripts\activate      # for Windows
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 🚀 Getting Started  

After setting up the environment, you can start exploring the language identification pipeline:

1. **Open the main notebook:**
   ```bash
   jupyter notebook main_notebook.ipynb
   ```
   Or if using VS Code, simply open `main_notebook.ipynb` in the editor.

2. **Run the cells sequentially:**
   - Start from the top and execute each cell in order
   - The notebook includes data loading, exploratory analysis, feature engineering, model training, and evaluation
   - Each section is clearly documented with markdown explanations

3. **Expected workflow:**
   - **Data Loading:** Load preprocessed corpora for all four languages
   - **EDA:** Explore dataset statistics and sample texts
   - **Feature Engineering:** Convert text to TF-IDF vectors
   - **Model Training:** Train multiple classifiers (Naive Bayes, Logistic Regression, SVM)
   - **Evaluation:** Compare model performance with metrics and visualizations




