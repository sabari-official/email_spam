# MACHINE LEARNING MODEL IMPLEMENTATION

**Email Spam Detection using Predictive Models**
--

---

**Company**     : CODETECH IT SOLUTIONS

**Name**        : SABARIVASAN E

**Intern ID**   : CTIS3748

**Domain**      : PYTHON PROGRAMMING

**Duration**    : 4 WEEKS

**Mentor**      : NEELA SANTHOSH

---

## **PROJECT OVERVIEW**

This project implements a machine learning-based email spam classification system using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization and Logistic Regression modeling. The interactive Jupyter notebook demonstrates the complete machine learning pipeline: data loading, exploratory data analysis, text feature extraction, model training, and comprehensive evaluation with confusion matrices and classification reports. The system is trained on 5,728 labeled emails (ham/spam) and achieves binary classification with detailed performance metrics.

---

## **TASK TYPE PERFORMED**

1. **Data Loading & Preprocessing** - CSV parsing, column renaming, label encoding (ham/spam → 0/1), missing value detection and handling
2. **Exploratory Data Analysis (EDA)** - Dataset shape analysis, class distribution visualization, missing value assessment, dataset statistics
3. **Text Vectorization** - TF-IDF feature extraction with configurable stop words, max document frequency filtering, sparse matrix generation
4. **Train-Test Splitting** - Stratified 80-20 split with random_state=42 for reproducible results, preserving class distribution
5. **Model Training & Evaluation** - Logistic Regression classifier with hyperparameter tuning, accuracy scoring, confusion matrix analysis, precision/recall/F1 computation

---

## **TOOLS AND RESOURCES USED**

| **Category** | **Tools & Technologies** |
|-------------|--------------------------|
| **Language** | Python 3.x |
| **Data Processing** | Pandas (DataFrames), NumPy (arrays) |
| **ML Framework** | Scikit-learn (sklearn) v1.x+ |
| **Text Vectorization** | TfidfVectorizer with English stop words |
| **Algorithm** | Logistic Regression (max_iter=1000) |
| **Visualization** | Matplotlib, Seaborn (confusion matrix heatmaps) |
| **Metrics** | Accuracy, Confusion Matrix, Classification Report |
| **Notebook** | Jupyter Notebook (.ipynb) with interactive cells |
| **Data Format** | CSV (5,728 emails with text & spam labels) |

---

## **EDITOR USED**

- **Visual Studio Code (VS Code)** - Jupyter notebook editing and execution
- **Jupyter Kernel** - Interactive cell execution with live output

---

## **APPLICABILITY & USE CASES**

1. **Email Security Systems** - Enterprise spam filtering and malicious email detection
2. **Email Service Providers** - Gmail, Outlook, Yahoo mailbox protection and automatic filtering
3. **Cybersecurity** - Phishing email detection and prevention systems
4. **Content Moderation** - Automated classification of user-generated content
5. **Data Science Education** - Foundational NLP and machine learning pipeline demonstration
6. **Document Classification** - Binary text classification for various document types
7. **Fraud Prevention** - Detecting suspicious or fraudulent communications
8. **Customer Communication** - Filtering unsolicited bulk emails and newsletters

---

## **PROJECT STRUCTURE**

```
Task-4/
├── spam_email.ipynb     (13 cells) - ML pipeline notebook
├── emails.csv           (5,728 emails) - Dataset
└── README.md            - Documentation
```

**Dataset**: 5,728 labeled emails (0=ham, 1=spam)

---

## **CODE CELLS EXPLANATION**

**Cells 1-5 (Data Preparation)** - Import libraries (pandas, numpy, sklearn, matplotlib); load emails.csv; rename columns to "label" and "message"; encode labels (ham→0, spam→1)

**Cells 6-9 (EDA & Cleaning)** - Inspect shape and dtypes; verify class distribution; handle missing values; ensure data quality

**Cell 10 (Train-Test Split)** - Stratified 80-20 split (4,582 train, 1,146 test); preserves class ratio; uses random_state=42 for reproducibility

**Cell 11 (TF-IDF Vectorization)** - Converts text to sparse matrix; removes English stop words; ignores terms in >90% documents; produces ~7,000+ features

**Cell 12 (Model Training)** - Logistic Regression with max_iter=1000; learns from training data

**Cells 13-16 (Evaluation)** - Prediction on test set; computes accuracy; generates confusion matrix heatmap; displays precision/recall/F1-score

---

## **EXECUTION FLOW**

1. Import libraries
2. Load emails.csv
3. Prepare & clean data
4. Split 80-20 with stratification
5. Vectorize text (TF-IDF)
6. Train Logistic Regression
7. Predict on test set
8. Evaluate: accuracy, confusion matrix, classification report

---

## **KEY TECHNICAL FEATURES**

- **Stratified Sampling**: Maintains class balance in train-test split
- **TF-IDF Weighting**: Automatic feature importance without manual engineering
- **Sparse Matrices**: Memory-efficient high-dimensional text representation
- **Comprehensive Metrics**: Accuracy, precision, recall, F1-score analysis
- **Confusion Matrix**: Visual identification of false positives/negatives
- **Reproducible**: Fixed random_state ensures identical results
- **Interactive**: Step-by-step cell execution with live output
