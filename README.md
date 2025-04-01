# 🧠 Machine Learning for Stroke Prediction  
**Can We Detect Stroke Before It Strikes?**

## 👩‍⚕️ Project Overview

This project explores how machine learning can support **early stroke risk prediction**, especially in real-world settings where data is limited, imbalanced, and privacy-constrained. We used models like **Random Forest, LightGBM**, and **XGBoost** to classify stroke cases and identify key risk factors.

## 🎯 Goals

- Build ML models that work well on **small, privacy-restricted datasets** without overfitting.
- Improve **interpretability** to support clinical decision-making.
- Address **class imbalance** to minimize false negatives.
- Optimize for **real-time hospital deployment**.

## 🗂️ Dataset

- **Source:** [Kaggle – Stroke Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)
- **Size:** 4,909 records
- **Features:** Age, gender, hypertension, heart disease, average glucose level, BMI, smoking status, work type, etc.

> ⚠️ Only 4% of patients had a stroke, making class imbalance a major challenge.

## 🧪 Methods

- **Preprocessing:** Null handling, outlier detection, one-hot encoding, robust scaling
- **Modeling:** Logistic Regression, Random Forest, XGBoost, LightGBM
- **Evaluation:** Precision, Recall, F1-score, AUC–ROC, Confusion Matrix
- **Feature Selection:** Full vs. reduced feature sets
- **Threshold Tuning:** Prioritize recall to reduce false negatives

## 📈 Key Insights

- **Age** was the most predictive feature, followed by **glucose level**, **BMI**, and **hypertension**.
- **Former smokers** were more vulnerable than current smokers.
- **Self-employed** individuals showed higher stroke risk.
- **Heart disease** and **hypertension** increased stroke odds by 5.24x and 4.44x, respectively.

## ✅ Final Model

| Model          | Dataset | Threshold | Reasoning                           |
|----------------|---------|-----------|-------------------------------------|
| Random Forest  | Full    | 0.4       | Balanced recall, accuracy, and cost |

## 🚀 Deployment Considerations

- Deployable in **hospital EHR systems**
- Compatible with **wearable devices** for continuous monitoring
- Explore **federated learning** for privacy-preserving training
- Maintain **HIPAA/GDPR compliance**

## 🎬 Poster Video

Watch our video presentation here:  
[📺 YouTube Link – Presentation](#) *(https://www.youtube.com/watch?v=FsRFX6VEKMc)*

## 📎 Authors

- **Ngoc (Martius) Nguyen**  
- **Phan Anh Nguyen**  
*Georgia State University – J. Mack Robinson College of Business*

---

## 📚 References

1. Soriano, F. (2021). *Stroke Prediction Dataset.* [Kaggle](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)  
2. WHO (2024). *Global Health Estimates: Stroke Statistics*  
3. CDC (2024). *Stroke Facts and Economic Impact*  
4. AHA (2024). *Heart Disease and Stroke Update*
