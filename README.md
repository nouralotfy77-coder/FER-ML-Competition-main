# 🏆 FER-ML Competition Rules

Welcome to the **FER-ML Competition**!  
Please read the following rules carefully before participating.  
These rules ensure fair play and maintain the integrity of the leaderboard.

---

## 🧩 Objective

Develop a **machine learning model** that accurately classifies human facial expressions using the **FER-2013 dataset**.  
Your goal is to maximize **classification accuracy** on the **hidden private test set**.

---

## 🗂 Dataset Information

- The dataset is derived from **[FER-2013](https://www.kaggle.com/datasets/deadskull7/fer2013)**.  
- It contains 48×48 grayscale facial images labeled with one of seven emotions:
  - 0 → Angry  
  - 1 → Disgust  
  - 2 → Fear  
  - 3 → Happy  
  - 4 → Sad  
  - 5 → Surprise  
  - 6 → Neutral



### Public Files:
the dataset is hosted externally on **Google Drive**.

### 🔗 **Download Link**
➡️ [Click here to access the dataset](https://drive.google.com/drive/folders/1xyPHM1E1YMBFJ6pc0jg4brhvNi_vUcCJ?usp=sharing)

### Private Files:
- Test_data → Hidden ground-truth data used for automatic evaluation  

---

## 🧠 Model Requirements

Participants must use **machine learning models** (e.g., Random Forest, SVM, Logistic Regression, etc.).  
Deep learning models (CNNs, transformers, etc.) may be used **only if implemented locally** — no pretrained weights or external datasets allowed.

---

## ⚙️ Submission Guidelines

1. Train your model using `data/train.csv`.
2. Predict labels for the samples in `data/test.csv`.
3. Save your predictions as `submissions/submission.csv` in the format:

   | id | predicted_label |
   |----|-----------------|
   | 0  | 3               |
   | 1  | 0               |
   | 2  | 6               |

4. Create a **Pull Request (PR)** with your submission file.  
5. The **GitHub Actions** workflow will automatically evaluate your submission using the hidden private test labels.

---

## 🧮 Evaluation Metric

- Metric: **Accuracy**
- The evaluation script compares your `predicted_label` values with the hidden ground truth.
- The result will appear automatically in your Pull Request **Checks tab**.

---

## 🚫 Restrictions

To ensure fairness:
- ❌ No external labeled data  
- ❌ No manual tuning based on private test feedback  
- ❌ No submission of multiple models in a single PR  
- ❌ No use of pretrained deep learning models unless approved  

---

## 🕐 Submission Limits

- Each Team should name the file something like: **Team1**.
- Only the **latest submission** counts toward the leaderboard.

---

## 🧾 Leaderboard

- Leaderboard scores are automatically updated based on accuracy.
- In case of identical scores, the earlier submission time will be used as a tiebreaker.

---

## 📩 Contact

If you face issues with the repository or evaluation: 
- Contact me at tasneem.mselim@gmail.com 

---

Good luck, and happy modeling! 🚀  
**Let the best model win!**
