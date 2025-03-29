# AI-Security-and-Privacy
# Supervised Learning-Based Attack Classifier

This project was completed as part of CYSE 635: Machine Learning for Cybersecurity at Old Dominion University.
</br>The objective was to build a supervised learning model to classify attack and benign logs using various machine learning algorithms.

---

## 📊 Project Summary

The assignment focused on developing a classifier using a combination of benign, jamming, and spoofing signal logs. The models were trained to distinguish between benign and malicious logs using features extracted from signal data.

---

## 🧠 Algorithms Used

- **K-Nearest Neighbors (KNN)**
- **Logistic Regression**
- **Support Vector Machine (SVM)** (for comparison)

Each model was evaluated using confusion matrices to measure:
- True Positives (TP)
- True Negatives (TN)
- False Positives (FP)
- False Negatives (FN)

---

## 📁 Project Structure

- `/Main.ipynb` – Main Jupyter Notebook with code and model training
- `/Report/Supervised_Learning_Base_Attack_Classifier.pdf` – Formal write-up of the project
- `/Data/` – Contains the original CSV logs used for training/testing
  - `benign_log.csv`
  - `jamming_log.csv`
  - `spoofing_log.csv`
- `LICENSE` - MIT License
- `README.md` - This file

---

## 🧼 Preprocessing & EDA
- Categorical encoding using `LabelEncoder`
- Combined datasets into a unified format
- Exploratory Data Analysis:
  - Histograms for feature distribution
  - Pie charts for class distribution (benign vs attack)
- Data split into training and test sets for evaluation

---

## 📈 Results Overview

- **KNN** outperformed other models in identifying attack types and minimizing misclassifications
- **Logistic Regression** had higher false negatives
- **SVM** misclassified more benign signals as attacks

Each model brought out trade-offs between sensitivity and specificity, showcasing real-world ML behavior in cybersecurity.

---

## 🧪 Tools & Libraries

- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

## 🔒 License

This project is licensed under the [MIT License](LICENSE).

---

## 👨‍💻 Author

**Sahad Rafiuzzaman**  
Graduate Student – Cybersecurity
Graduate Student - Data Science & Analytics
Old Dominion University
