

# Predictive Modeling of Mental Health Trends using Natural Language Processing on Patient Notes

A research-based Natural Language Processing framework for detecting and predicting mental health conditions from patient narratives, clinical notes, and diary entries using hybrid machine learning and deep learning models.

This project was developed as part of the **M.Tech (Computer Science and Engineering – Business Analytics)** program at **Vellore Institute of Technology (VIT), Chennai**.

---

# Abstract

Mental health disorders represent a growing global public health concern. However, early identification remains difficult because much of the relevant information exists in **unstructured textual data** such as clinical notes, therapy transcripts, patient diaries, and electronic health records.

This project proposes a **predictive modeling framework using Natural Language Processing (NLP)** to analyze patient narratives and identify mental health trends. Unlike traditional approaches that rely on a single dataset, this system integrates **multiple heterogeneous datasets**, including synthetic clinical notes, patient diaries, journal entries, and emotion-labeled corpora.

The framework includes:

* Text preprocessing and PHI masking
* Contextual embedding generation using **MiniBioBERT**
* Hybrid modeling using **transformers, LSTM/BiLSTM networks, and ensemble machine learning methods**
* Explainable AI techniques for interpretability

The proposed system achieves improved classification accuracy while providing **clinically interpretable insights**, supporting the development of AI-powered mental health decision-support systems.

---

# Problem Statement

Mental health diagnosis typically relies on **subjective patient reports and clinical observations**, making large-scale monitoring and early detection challenging.

Although vast amounts of mental health information exist in **unstructured textual narratives**, analyzing these data sources manually is:

* Time-consuming
* Error-prone
* Difficult to scale

Therefore, there is a need for a **data-driven, automated, and interpretable system** that can extract meaningful psychological signals from patient text data.

---

# Key Objectives

* Develop an NLP-based predictive framework for mental health analysis
* Integrate multiple heterogeneous datasets for improved model generalization
* Extract semantic and emotional features from patient narratives
* Implement hybrid machine learning and deep learning models
* Provide interpretable predictions using explainable AI techniques
* Enable early detection and monitoring of mental health conditions

---

# Datasets Used

The system integrates **six heterogeneous datasets** collected from Kaggle, including:

* Synthetic clinical notes
* Patient diaries
* Personal journal entries
* Mental health discussion data
* Emotion-labeled text datasets
* Augmented clinical note datasets

Combining multiple datasets improves **linguistic diversity, emotional variability, and model robustness**.

---

# NLP Processing Pipeline

The system follows a structured NLP workflow.

### 1. Data Collection

Data is collected from multiple textual sources such as:

* Clinical notes
* Patient diaries
* Mental health datasets
* Social media emotional text corpora

---

### 2. Data Preprocessing

Text preprocessing improves data quality and consistency.

Steps include:

* Text cleaning
* Tokenization
* Lemmatization
* Stopword removal
* PHI masking (removal of sensitive personal information)
* Label normalization

---

### 3. Feature Extraction

Multiple feature representations are used to capture linguistic and emotional patterns.

#### TF-IDF

Captures term importance within documents.

#### Word2Vec

Learns semantic word relationships.

#### MiniBioBERT Embeddings

Generates **contextual biomedical language embeddings** suitable for healthcare text.

#### Sentiment Features

Extracts emotional polarity using sentiment analysis.

All features are **combined into a unified feature representation**.

---

# Machine Learning Models

The system evaluates both **traditional and deep learning models**.

### Traditional Models

* Logistic Regression
* Random Forest
* XGBoost

---

### Deep Learning Models

* LSTM (Long Short-Term Memory)
* BiLSTM (Bidirectional LSTM)

These models capture **temporal and contextual dependencies** in patient narratives.

---

# Hybrid Ensemble Model

A hybrid ensemble classifier combines:

* Logistic Regression
* Random Forest

This improves classification robustness by leveraging both **linear and nonlinear decision boundaries**.

---

# Explainable AI

To improve clinical trust and interpretability, the system integrates **Explainable AI techniques**, including:

* Attention visualization
* Feature importance analysis
* SHAP-based explanations (optional)

These methods help clinicians understand **which words or linguistic signals influenced the prediction**.

---

# Mental Health Categories Detected

The model classifies text into multiple mental health conditions:

* Anxiety
* Bipolar Disorder
* Depression
* Stress
* Personality Disorder
* Suicidal Tendencies
* Normal

---

# Model Performance

### Overall Model Comparison

| Model                  | Accuracy | Precision | Recall   | F1 Score |
| ---------------------- | -------- | --------- | -------- | -------- |
| Logistic Regression    | 0.74     | 0.74      | 0.74     | 0.73     |
| Random Forest          | 0.73     | 0.74      | 0.73     | 0.72     |
| LSTM                   | 0.72     | 0.71      | 0.72     | 0.69     |
| BiLSTM                 | 0.68     | 0.59      | 0.68     | 0.63     |
| **Ensemble (LR + RF)** | **0.76** | **0.76**  | **0.76** | **0.75** |

The **ensemble model achieved the best performance**.

---

# ROC-AUC Performance

| Class                | ROC-AUC |
| -------------------- | ------- |
| Anxiety              | 0.9652  |
| Bipolar              | 0.9541  |
| Depression           | 0.9018  |
| Normal               | 0.9777  |
| Personality Disorder | 0.9450  |
| Stress               | 0.9436  |
| Suicidal             | 0.9203  |

---

# Technologies Used

Programming & Frameworks

* Python
* PyTorch
* Scikit-learn
* HuggingFace Transformers
* Gensim
* NLTK

Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn

NLP Models

* TF-IDF
* Word2Vec
* MiniBioBERT
* LSTM / BiLSTM

---

# Applications

This system can be used in:

* Mental health monitoring systems
* AI-based clinical decision support
* Early suicide risk detection
* Psychological research analytics
* Healthcare data intelligence platforms

---

# Future Work

Future improvements include:

* Temporal modeling for longitudinal mental health tracking
* Multimodal analysis (text + voice + facial expression)
* Federated learning for privacy-preserving training
* Real-time mental health monitoring systems

---

# Author

**Surya M S**
M.Tech Integrated – Computer Science and Engineering (Business Analytics)
Vellore Institute of Technology, Chennai

Supervisor
Dr. Jeipratha P N
