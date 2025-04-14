# Student Loan Credit Risk Prediction using Deep Learning

## 📌 Goal

The objective of this project is to build a deep learning model that predicts the **credit risk of student loan applicants** based on various academic, financial, and personal background features. This model aims to assist lenders in identifying reliable borrowers and minimizing default risk by evaluating predictive patterns in student profiles.

## 🧠 Problem Statement

Student loans are one of the largest forms of consumer debt in the United States, and identifying students who are less likely to default can help institutions manage risk more effectively. The goal is to determine whether a student is a good or bad credit risk using features like payment history, GPA ranking, financial aid score, workshop performance, and more.

## 🧪 Dataset Overview

The dataset includes the following key features:
- `payment_history`: Score indicating consistency of past payments
- `finance_workshop_score`: Score from financial literacy training
- `gpa_ranking`, `cohort_ranking`: Indicators of academic performance
- `alumni_success`: Proxy for school reputation or network effect
- `study_major_code`: Encoded major of study
- `time_to_completion`: Duration in months to complete the program
- Other contextual financial and academic indicators

The target variable is a binary classification: **good credit risk (1)** or **bad credit risk (0)**.

## ⚙️ How to Run (Coming Soon)

Instructions on how to clone the repository, install dependencies, and run the model will be added soon.

## 📈 Results & Insights

- The trained model successfully outputs probability predictions between 0 and 1, indicating the likelihood of good credit risk.
- For example, one test prediction returned `0.974`, showing 97.4% confidence the student is a good credit risk. The corresponding student had:
  - High `finance_workshop_score` (0.99)
  - Strong `payment_history` (7.1)
  - Good `cohort_ranking` (3.3)
  - On-time program completion (`24 months`)
- These types of features appear to be highly influential in predicting good credit outcomes.
- Minor differences in prediction results when compared to the instructor’s notebook may arise due to different initial weights, random states, or slight architecture variations.

## 📌 Unique Observations

- `finance_workshop_score` and `payment_history` seem to have a strong correlation with the model's confidence.
- Even with low `stem_degree_score`, students with good financial literacy and academic performance were still classified as low-risk.
- Predictions are probabilistic, offering flexibility for threshold tuning based on business needs (e.g., 0.6 instead of 0.5).

## 📚 Resources & Citations

- TensorFlow and Keras libraries were used to create, train, and evaluate the deep learning model.
- Data scaling was applied using `StandardScaler` from scikit-learn.
- No external datasets were used beyond the course-provided one.
- Any instructional references or modeling frameworks were inspired by Deep Learning Bootcamp/Instructor-led Jupyter notebooks.

## ✅ Conclusion

This project demonstrates that deep learning can be a powerful tool in evaluating student credit risk using academic and financial indicators. The model shows promising accuracy and interpretable prediction outputs, paving the way for further optimization, feature engineering, and real-world implementation.
