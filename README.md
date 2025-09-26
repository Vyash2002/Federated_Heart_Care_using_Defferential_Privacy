### Federated Heart-Care using Differential Privacy

📌 Overview

Heart disease is a leading cause of mortality worldwide. This project leverages Federated
Learning (FL) and Differential Privacy (DP) to build a privacy-preserving heart disease
prediction system.

Instead of centralizing sensitive patient data, the system enables multiple healthcare institutions
to collaboratively train models while ensuring data confidentiality. Streamlit provides an
interactive dashboard for real-time predictions and visualizations.

✨ Features

1. Federated Learning Framework: Collaborative model training across multiple clients
(simulated hospitals) without sharing raw patient data.

2. Differential Privacy Integration: Uses DP-SGD (via Opacus) to add noise and
guarantee privacy.

4. Machine Learning Models: Logistic Regression, SVM, Random Forest, and ANN.

5. Visualization & EDA: Feature importance, confusion matrices, accuracy graphs, etc.

6. Interactive Streamlit Dashboard:
   
    ○ Upload datasets (.csv, .xlsx)
  
    ○ Configure privacy parameters (noise multiplier, clipping norm)
  
    ○ Visualize training and evaluation metrics
  
    ○ Predict heart disease risk for new patients in real-time
  
🏗️ System Architecture

1. Data Preprocessing
   
    ○ Missing value handling

    ○ Feature encoding & normalization
  
    ○ Class balancing (SMOTE)

3. Model Training
   
    ○ Centralized ML models for baseline accuracy

    ○ ANN implementation in PyTorch
  
    ○ Federated Averaging (FedAvg) for aggregation

5. Differential Privacy
   
    ○ Gradient clipping

    ○ Gaussian noise addition
  
    ○ Privacy budget tracking (ε, δ)

7. Deployment
   
    ○ Streamlit dashboard for clinicians and researchers

    ○ API/Edge deployment support for healthcare systems

⚙️ Tech Stack

1. Programming Language: Python 3.11

2. Libraries & Tools:
   
     ○ Data Processing: pandas, numpy
  
     ○ Visualization: matplotlib, seaborn
  
     ○ Machine Learning: scikit-learn, imbalanced-learn
  
     ○ Deep Learning: PyTorch, Opacus
  
     ○ Federated Learning: Custom FL + FedAvg
  
     ○ Web App: Streamlit
  
📊 Results

1. Baseline Accuracy:
   
    ○ Logistic Regression → 74.94%
  
    ○ SVM → 91.56%
  
    ○ Random Forest → 97.19%
  
3. Centralized ANN → 89.26%

4. Federated Learning with DP → ~96% accuracy with minor privacy-utility trade-off

5. Streamlit Dashboard → Enabled real-time predictions and visualization of training
progress
