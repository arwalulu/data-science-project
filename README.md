# Data-Driven Intrusion Detection in IoT Networks  
**Course:** Data Science (CS307)  
**Students:**  
- Arwa Alomari  
- Dalia Guail  
- Mohamed Albarazi  

---

## 📌 Project Overview  
This project builds a **data-driven Intrusion Detection System (IDS)** for IoT networks using machine learning.  
We analyze real IoT network traffic, clean and preprocess the data, handle imbalance, select the most important features, and evaluate multiple ML models to detect cyberattacks such as DoS, DDoS, Malware, PortScan, and MITM.

The full workflow includes:  
- Data cleaning  
- Handling missing and infinite values  
- SMOTE oversampling  
- Feature selection (SelectKBest – top 15 features)  
- Normalization (StandardScaler)  
- Training 12+ ML models  
- Evaluation using Accuracy, Precision, Recall, F1-score, and Confusion Matrix  
- SHAP feature importance for interpretability  

---

## 📂 Notebook  
The full implementation is available in:  
**`DataSCProject.ipynb`**

---

## 📊 Dataset  
Due to size limits, the dataset is **not uploaded to GitHub**.  
You can download it from the official source:

🔗 **CIC IoT Dataset 2023:**  
https://www.unb.ca/cic/datasets/iotdataset-2023.html

---

## 📝 Outcomes  
You may attach the result screenshots in the repo (e.g., under `/results/` folder).  
Key findings:

- **Best-performing models:**  
  - Random Forest  
  - Extra Trees  
  - Linear Discriminant Analysis (LDA)  
  - LightGBM  
  These models reached **~88–90% accuracy**, with strong precision, recall, and F1.

- **Moderate models:**  
  - KNN, Ridge, Decision Tree  

- **Lower-performing models:**  
  - Logistic Regression  
  - Naïve Bayes  
  - AdaBoost  
  - Linear SVC  

- **Preprocessing impact:**  
  - SMOTE improved recall for minority attack classes  
  - StandardScaler stabilized model training  
  - Feature selection reduced dimensionality and improved performance  

---

## 🧠 Discussion & Analysis  
- The dataset presented **severe class imbalance**, making rare attacks much harder to detect. SMOTE was essential to improve model fairness across classes.  
- Feature selection significantly reduced noise and improved generalization, especially for linear and ensemble models.  
- Tree-based models (Random Forest, Extra Trees, Gradient Boosting) performed best because they handle **non-linear and high-dimensional data** effectively.  
- SHAP feature analysis increased interpretability by highlighting which traffic features contribute most to attack detection.  
- Limitations include some misclassification of rare attacks and lack of real-time evaluation.  

**Future improvements:**  
- Deploy in a real-time pipeline  
- Try deep learning (LSTM, CNN) for sequence-based traffic patterns  
- Improve handling of extremely rare attack types using cost-sensitive learning  
- Add live monitoring dashboards  

---

## ✔️ How to Run  
1. Download or clone the repo  
2. Install required libraries (listed at the top of the notebook)  
3. Download the dataset from the link  
4. Update the dataset path in the notebook  
5. Run all cells  

---

If you want, I can also make a **shorter README**, a **prettier version with emojis**, or a **professional academic version**.

