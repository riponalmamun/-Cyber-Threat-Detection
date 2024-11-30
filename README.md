# 🚀Cyber Threat Detection


# About Dataset:

The Cyber Threat Detection dataset is a simulated dataset designed for developing and testing federated learning-based cyber threat detection models. This dataset is tailored for research and experimentation in distributed anomaly detection and privacy-preserving cybersecurity frameworks. It includes traffic features commonly used in intrusion detection systems (IDS) with a focus on cloud and edge computing environments. Each record represents network traffic metadata, with labeled instances of both normal and malicious activities, making it ideal for machine learning applications in cybersecurity.

# Dataset Features:

The dataset consists of 1,430 instances, with 23 features including information on packet size, duration, bytes sent/received, flow statistics, and attack labels. It covers common cyberattacks such as DDoS, Brute Force, and Ransomware, along with normal network traffic.


#🚀Cyber Threat Detection Analysis

               
               
               
# Abstract

Analysis of Cyber Threat Detection dataset led to build advanced machine learning models for intrusion handling in cloud and edge computing. Implementation of multiple ensemble methods like Random Forest, XGBoost, stacking envois and Voting Classifiers gave perfect classification metrics (Accuracy, Precision, Recall & F1-Score of 1 for cross validation). We used Explainable AI (XAI) methods like SHAP Label and LIME to get insights on the models’ predictions, what are the top features affecting the result. Since the results confirm the simplicity and separability of the features in the dataset, it is suggested for future validation in order to obtain a more reliable result, without any data leakage or overfitting. The value of ensemble learning in cybersecurity and necessity of XAI for interpretability is casted here by this study.

# Introduction

The increasing number of vulnerabilities to cyber threat has mainly been fueled by the ascent of cloud and edge computing, converting effective intrusion detection systems (IDS) required. Machine learning models, especially ensemble approaches promise to provide a solution by exploiting data patterns that can be used for detecting/protecting the attacks. Cyber Threat Detection dataset is such simulation of network activity against which we evaluate our methodologies. The work aims to construct high performance ensemble classifiers for the Intrusion Detection (ID) and use Explainable AI (XAI) techniques to explain the decision of these models. It also stresses the need for trustworthy testing to validate obtained results.

# Methodology 

1. Dataset Overview

The CyberFedDefender dataset contains 1,430 instances and 23 features, including numerical attributes like Bytes Sent, Packets Received, and Duration. The target variable (Label) identifies normal (0) and attack (1) instances.

3. Data Preprocessing
   
•	Data Cleaning: Removed irrelevant features (Timestamp, Source IP, Destination IP) and verified no missing values.

•	Feature Scaling: Standardized numerical features using StandardScaler.

•	Handling Imbalance: Applied SMOTE (Synthetic Minority Oversampling Technique) to address class imbalance.

5. Model Implementation


# Four ensemble models were evaluated: 

1.	Random Forest: Bagging-based method for high accuracy and stability.
   
3.	XGBoost: Gradient boosting framework for handling complex relationships.
   
5.	Stacking Classifier: Combined Random Forest and XGBoost with Logistic Regression as the meta-model.
   
7.	Voting Classifier: Combined multiple classifiers using hard and soft voting.
   
4. Explainable AI (XAI)
   
•	SHAP: Used for global and local feature importance analysis.

•	LIME: Provided instance-specific explanations for individual predictions.
 
 
 # 6. Evaluation Metrics 
   
 **Performance was assessed using: **

•	Accuracy

•	Precision

•	Recall

•	F1-Score


All models achieved perfect metrics, suggesting a dataset with high feature separability or potential issues like data leakage or overfitting.

 
# Explainable AI Analysis 

1.	SHAP Results:
   
Global Importance: Features such as Bytes Sent, Packets Received, and Duration were the most influential in distinguishing between normal and attack instances.

Local Explanations: Individual predictions were attributed to specific feature values, providing transparency in decision-making.

2.	LIME Results:
   
	Instance-specific predictions revealed which features strongly influenced classification outcomes, enhancing interpretability.


# Discussion 

While the results are highly promising, achieving perfect scores across all models warrants caution. Potential reasons include:

Dataset Simplicity: Clear class separability.

Data Leakage: Unintended inclusion of target-related information.

Overfitting: Over-optimization on a limited dataset.

Further testing on unseen data and increasing dataset complexity are recommended to validate the generalizability of these results.

# Conclusion

Using the Cyber Threat Detection dataset, this study efficiently employed ensemble learning methods for intrusion detection. The perfect classification metrics show the power of ensemble models but also emphasizes the necessity of further validations for these perfect metrics. SHAP (explainable AI tool): LIME both, explained the feature importance in-depth and enhanced the interpretability of model from the possible follow-up work, we suggest thorough testing of robustness with more complex datasets and adversarial scenarios practitioners in mind.


GitHub Link: https://github.com/riponalmamun/-Cyber-Threat-Detection

Dataset Link: https://www.kaggle.com/datasets/hussainsheikh03/cyber-threat-detection







