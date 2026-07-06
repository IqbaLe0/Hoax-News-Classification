# 🧠 Hoax News Detection (Indonesian Language)

Project klasifikasi berita hoaks vs faktual menggunakan pendekatan **Sentence-BERT embedding + Tree-Based Machine Learning Models** (LightGBM, XGBoost, CatBoost).

---

## 🚀 Overview

Proyek ini merupakan pipeline end-to-end untuk mendeteksi berita hoaks dalam bahasa Indonesia dengan memanfaatkan:

- **Semantic Text Embedding** (Sentence-BERT multilingual)
- **Machine Learning berbasis tree ensemble**
- **Hyperparameter tuning (Optuna)**
- **Evaluasi model komprehensif**

Tujuan utama:
> Mengklasifikasikan apakah suatu berita termasuk **hoaks atau faktual** berdasarkan isi teks secara semantik, bukan sekadar keyword matching.

---

## 📊 Dataset

Dataset yang digunakan pada proyek ini berasal dari Kaggle.

### 📌 Kaggle Dataset
- Dataset utama diambil dari Kaggle:  
  [https://www.kaggle.com/datasets/xxxx/xxxx](https://www.kaggle.com/datasets/linkgish/indonesian-fact-and-hoax-political-news)

### ✅ Kelas Faktual (Label 0)
- CNN Indonesia (`dataset_cnn_10k.xlsx`)
- Kompas (`dataset_kompas_4k.xlsx`)
- Tempo (`dataset_tempo_6k.xlsx`)

### ❌ Kelas Hoaks (Label 1)
- TurnBackHoax (`dataset_turnbackhoax_10k.xlsx`)

### Kolom utama yang digunakan:
- `Title`
- `FullText`

---

## 🧪 Pipeline Workflow

1. 📥 Data Loading & Integration  
2. 🧹 Text Preprocessing  
3. 🔡 Sentence-BERT Embedding (Multilingual)  
4. ✂️ Train-Test Split (Stratified 80:20)  
5. 🌳 Model Training:
   - LightGBM
   - XGBoost
   - CatBoost  
6. ⚙️ Hyperparameter Tuning (Optuna)  
7. 📈 Evaluation:
   - Accuracy
   - Precision
   - Recall
   - F1-score  
8. 📊 Model Comparison  
9. 📉 Visualization (Confusion Matrix, Metrics)  
10. 💾 Model Saving & Inference Pipeline  

---

## 🤖 Models Used

| Model      | Description |
|------------|-------------|
| LightGBM   | Gradient boosting framework yang cepat dan efisien |
| XGBoost    | Optimized gradient boosting dengan regularization |
| CatBoost   | Robust terhadap categorical features dan overfitting |

---

## 🧠 Text Representation

Menggunakan:

- **Sentence-BERT (SBERT) Multilingual Model**
  - Menangkap makna semantik teks
  - Lebih kuat dibanding TF-IDF / Bag-of-Words
  - Cocok untuk bahasa Indonesia

---

## 📈 Evaluation Metrics

Model dievaluasi menggunakan:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---
