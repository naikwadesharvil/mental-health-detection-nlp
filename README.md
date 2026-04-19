# 🧠 Explainable Transformer-based Detection of Depression & Anxiety

## 🎯 Project Overview
This project explores detecting early signs of depression and anxiety from social media text using NLP and deep learning models.

We compare traditional machine learning, deep learning, and transformer-based approaches, with a focus on **interpretability using LIME** for clinically meaningful insights.

---

## 🔬 Research Questions
- Can transformer models outperform traditional ML methods in mental health classification?
- How do LSTM, BERT, and RoBERTa compare in performance and efficiency?
- Can LIME explanations provide interpretable insights for predictions?

---

## 📊 Current Progress (Day 3 ✅)

### Baseline Model
- TF-IDF + Logistic Regression
- Stratified train/val/test split (80/10/10)
- Class imbalance handled using `class_weight='balanced'`

### 📈 Results (Validation)
- Accuracy: **88.15%**
- Precision: **89.45%**
- Recall: **82.75%**
- F1 Score: **85.97%**
- ROC-AUC: **0.955**

---

## 📊 Methodology

### Dataset
- Twitter Suicidal Intention Dataset (current)
- Planned: Reddit Mental Health Dataset

### Models
- ✅ Baseline: TF-IDF + Logistic Regression
- 🔄 Next: LSTM (with attention)
- 🔄 Next: BERT-base fine-tuning
- 🔄 Next: RoBERTa-base fine-tuning

### Explainability
- 🔄 LIME (Local Interpretable Model-Agnostic Explanations)

### Evaluation Metrics
- Accuracy
- Precision / Recall
- F1-score
- ROC-AUC

---

## 📁 Repository Structure

project/
│
├── notebooks/
│ └── day3_baseline.ipynb
│
├── models/
│ ├── tfidf_vectorizer.joblib
│ └── logreg_tfidf.joblib
│
├── results/
│ └── metrics/
│ └── tfidf_logreg_val_metrics.json


---

## 🧠 Key Insights
- Strong baseline achieved with ROC-AUC > 0.95
- Model shows slightly lower recall for depressed class → improvement needed
- TF-IDF baseline provides a solid benchmark before deep learning

---

## 🔜 Next Steps
- Implement LSTM model (Day 4)
- Fine-tune BERT and RoBERTa
- Add LIME-based explainability
- Compare models on performance + interpretability

---

## 🛠️ Tech Stack
- Python
- Scikit-learn
- PyTorch
- Hugging Face Transformers
- LIME
- Pandas, NumPy, Matplotlib, Seaborn

---

## 👤 Author
Sharvil Naikwade  
B.Tech - Artificial Intelligence & Machine Learning  
Rajarambapu Institute of Technology (RIT)

---

## 📜 License
MIT License

---

## 🙏 Acknowledgments
- Hugging Face (transformers)
- Open-source NLP community
- Dataset contributors
