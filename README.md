# 📚 Data Integration Project: Book Domain

This project focuses on data integration across three datasets in the **book domain**: Amazon, Goodreads, and Kindle. The objective is to address both **instance-level** and **schema-level** heterogeneity, design a mediated schema, match and align records, and evaluate entity resolution strategies.

---

## 📁 Project Structure

### `Datasets/`
Contains all the raw datasets downloaded from Kaggle:

- **[Dataset1_Amazon.xlsx](https://www.kaggle.com/datasets/abdulhamidadavize/top-100-best-selling-books-on-amazon-20092021)**  
  _Top 100 Best Selling Books on Amazon (2009–2021)_

- **[Dataset2_GoodReads.csv](https://www.kaggle.com/datasets/brzy56/goodreads-choice-awards-2023-best-books-of-2023)**  
  _Goodreads Choice Awards Best Books of 2023_

- **[Dataset3_Kindle.csv](https://www.kaggle.com/datasets/asaniczka/amazon-kindle-books-dataset-2023-130k-books)**  
  _Amazon Kindle Books Dataset 2023_

- **`mediated_schema.csv`** – Manually created mediated schema used to unify attributes across datasets

- **Ground Truth Files:**  
  - `amazon_max_GT.csv`, `amazon_weighted_avg_GT.csv`  
  - `goodreads_max_GT.csv`, `goodreads_w.avg_GT.csv`  
  - `kindle_max_GT.csv`, `kindle_weighted_GT.csv`

---

### `Implementation/`
Contains scripts and notebooks for schema matching, integration, and querying:

- `Matchers_Combiners.ipynb` – Matching & Combining strategies (Jaro-Winkler, SpaCy, TF-IDF, etc.)
- `Mediated_schema.ipynb` – Development of mediated schema
- `task.dl` – Datalog query scripts for answering competency questions

---

### `Reports/`
Detailed reports for each phase of the project:

- **`Report_Task_01.md`** –  
  - Dataset exploration and collection  
  - Competency question formulation  
  - Mediated schema design  
  - Structural and semantic heterogeneity analysis  

- **`Report_Task_02.md`** –  
  - Matcher implementation:  
    - Jaro-Winkler  
    - SpaCy Similarity  
    - TF-IDF + Cosine Similarity  
  - Combiner design: Max and Weighted Average  
  - Ground truth creation and evaluation using Precision, Recall, and F1 Score  

- **`Report_Task_03.md`** –  
  - XML schema parsing using ElementTree  
  - Schema tree generation for Data Source (DS) and Mediated Schema (MS)  
  - Similarity computation at node and path level using:  
    - Levenshtein Distance  
    - Jaccard Similarity  
    - TF-IDF + Cosine  
    - FuzzyWuzzy (Token Sort Ratio)  
  - Threshold-based alignment extraction and evaluation

---

## ✅ Tasks Completed

- ✅ Dataset collection from Kaggle  
- ✅ Mediated schema development  
- ✅ Competency question design  
- ✅ Implementation of multiple matchers:  
  - Jaro-Winkler  
  - SpaCy Similarity  
  - TF-IDF + Cosine Similarity  
  - Levenshtein Edit Distance  
  - Jaccard Similarity  
  - FuzzyWuzzy  
- ✅ Match result combination:  
  - Max combiner  
  - Weighted Average combiner  
  - Threshold selection  
- ✅ Ground truth preparation  
- ✅ Evaluation using Precision, Recall, and F1 Score  
- ✅ XML schema parsing with ElementTree  
- ✅ Schema tree generation (DS and MS)  
- ✅ Similarity matrices (node-level & path-level)  
- ✅ Threshold-based schema alignment extraction and evaluation

---

## 🛠 Technologies Used

- **Python** (pandas, scikit-learn, nltk, fuzzywuzzy, SpaCy)
- **ElementTree** (for XML schema parsing)
- **Jupyter Notebooks** (for exploration and implementation)
- **Datalog** (for expressing conjunctive queries)
- **Markdown** (for documentation and reports)

---

## 📌 Notes

This project demonstrates a practical pipeline for integrating heterogeneous book datasets, designing mediated schemas, resolving entities using different matchers and combiners, and evaluating alignment quality using standard metrics.

---

