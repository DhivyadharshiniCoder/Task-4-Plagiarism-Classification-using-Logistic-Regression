# 🧠 Task 4 – Plagiarism Classification using Logistic Regression

This task implements a binary classification model to identify plagiarism based on sentence similarity scores using Logistic Regression.

---

## 📁 Dataset

We used the `similarity_output_task3.csv` file generated from Task 3, which contains:

- `Sentence_File1`: Sentence from the first file
- `Sentence_File2`: Sentence from the second file
- `Similarity_Score`: Cosine similarity score between the sentences
- `Plagiarised`: Binary label (`1` = plagiarised, `0` = original)

---

## 🔍 Objective

Train a logistic regression classifier to predict whether a sentence pair is plagiarised based on the similarity score.

---

## 🛠️ Steps Followed

1. **Import and Preprocess Dataset**
2. **Split Data** into train and test sets (80-20)
3. **Train Logistic Regression Model**
4. **Evaluate** using:
   - Accuracy
   - F1 Score
   - Confusion Matrix
   - ROC Curve
   - AUC Score

---

## 📉 Evaluation Metrics

- ✅ Accuracy, Precision, Recall, F1-score (via `classification_report`)
- 📊 Confusion Matrix
- 📈 ROC Curve
- 🔵 AUC Score

---

## 🔁 Sigmoid Function (Model Logic)

Logistic Regression uses the **sigmoid function** to map input scores to probabilities:

\[
\sigma(x) = \frac{1}{1 + e^{-x}}
\]

Based on a default threshold of `0.5`, sentence pairs are classified as:
- `1` → **Plagiarised**
- `0` → **Original**

---

## ✅ Result

The model was successfully trained on semantic similarity scores and performed binary classification with high accuracy and AUC.

---

## 📦 Files Included

- `plagiarismchecker.ipynb` – Jupyter Notebook with full code
- `similarity_output_task3.csv` – Dataset used for training
- `README.md` – Project description
