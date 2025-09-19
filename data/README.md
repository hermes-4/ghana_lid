# 📂 Data Sources & Description

This folder contains information about the datasets and the preprocessing used for training and evaluating models in the project.  
Due to copyright and redistribution restrictions, some raw data files cannot be uploaded directly to GitHub.                         
However, the data obtained from these sources were preprocessed using the scrips in `data/preprocessing`. The cleaned and standardized corpora are stored in `data/processed`, each as a JSON file named by language (e.g., twi_corpus.json, ewe_corpus.json). These processed files are the ones used directly in training and evaluation.

---

### 📊 Data Sources

Ga
- **Source 1:** [Bible.com](https://www.bible.com/bible)  
- **Source 2:** [JW.org](https://www.jw.org)  

Dagbani
- **Source:** [JW.org](https://www.jw.org)  

Ewe
- **Source(s):** From a database named ewedictionarydb

Akan (Twi/Fante)
- **Source:** [TypeCraft Akan Corpus Release 1.0](https://www.researchgate.net/publication/323998547_TypeCraft_Akan_Corpus_Release_10)  


---

### ⚙️ Preprocessing

- Each language has its own preprocessing notebook in `data/preprocessing/`:
  - `akan_preprocessing.ipynb`
  - `dagbani_preprocessing.ipynb`
  - `ewe_preprocessing.ipynb`
  - `ga_preprocessing.ipynb`

Steps performed include:
1. Cleaning (removing unwanted characters, HTML tags, etc.)
2. Normalization (lowercasing, handling diacritics)
3. Tokenization
4. Saving cleaned text to JSON for model training



