# AI-Security-and-Privacy
## Data Poisoning Attack on Supervised Learning Models

This project was completed for CYSE 635: Machine Learning for Cybersecurity at Old Dominion University.  
It builds on a previous assignment to explore the impact of **data poisoning** on machine learning models trained to classify signal logs as either attack or benign.

---

## 🧪 Project Objective

The goal of this assignment was to demonstrate how injecting poisoned data into training sets can impact the performance of machine learning models in a cybersecurity context. By deliberately mislabeling a small portion of the dataset, this project simulates an adversarial attempt to reduce detection accuracy.

---

## 🧠 Models Evaluated

Three supervised learning models were trained on both clean and poisoned datasets:
- **K-Nearest Neighbors (KNN)**
- **Logistic Regression (LR)**
- **Support Vector Machine (SVM)**

Performance was assessed using confusion matrices to measure:
- True Positives (TP)
- True Negatives (TN)
- False Positives (FP)
- False Negatives (FN)

---

## 💉 Poisoning Methodology

- A small subset of attack and benign logs were intentionally mislabeled (100 examples total)
- These were injected into the training data to simulate a poisoning attack
- Models were retrained on the poisoned dataset and performance metrics were re-evaluated

---

## 📁 Project Structure

- `/Main.ipynb` – Main Jupyter Notebook with code and model training
- `/Report/Data_Poisoning_Attack_on_Artificial_Intelligence.pdf` – Formal write-up of the project
- `/Data/` – Contains the original CSV logs used for training/testing
  - `benign_log.csv`
  - `jamming_log.csv`
  - `spoofing_log.csv`
- `LICENSE` - MIT License
- `README.md` - This file

---

## 📈 Results Summary

| Model | Data | TN | FP | FN | TP |
|-------|------|----|----|----|----|
| KNN   | Clean     | 55 | 0  | 0  | 67 |
| KNN   | Poisoned  | 54 | 1  | 0  | 67 |
| LR    | Clean     | 55 | 0  | 67 | 0  |
| LR    | Poisoned  | 38 | 17 | 7  | 60 |
| SVM   | Clean     | 0  | 55 | 0  | 67 |
| SVM   | Poisoned  | 0  | 55 | 0  | 67 |

- **KNN** showed minimal changes with only one new false positive
- **Logistic Regression** was the most impacted, showing significant drop in accuracy
- **SVM** remained unaffected, demonstrating resilience to the poisoned data in this case

---

## 🔬 Tools & Libraries

- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## 🔒 License

This project is licensed under the [MIT License](LICENSE).

---

## 👨‍💻 Author

**Sahad Rafiuzzaman**  
Graduate Student – Cybersecurity  
Graduate Student – Data Science & Analytics 
Old Dominion University
