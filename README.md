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

