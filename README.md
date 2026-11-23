# 🇧🇩 Bangladesh Psychosocial and Behavioral Health Survey Dataset

<p align="center">

**A Survey-Based Dataset for Depression-Related Research and Explainable Artificial Intelligence**

[![Dataset](https://img.shields.io/badge/Dataset-507%20Responses-blue)]()
[![Format](https://img.shields.io/badge/Format-CSV-orange)]()
[![Python](https://img.shields.io/badge/Python-Jupyter%20Notebook-yellow)]()
[![Research](https://img.shields.io/badge/Research-Mental%20Health-purple)]()
[![XAI](https://img.shields.io/badge/Explainable%20AI-SHAP-green)]()

</p>

---

## 📌 Overview

This repository provides a structured survey-based dataset containing **507 valid responses** collected from individuals in the Sylhet and Rajshahi regions of Bangladesh during May–June 2026.

The dataset focuses on the relationship between psychosocial well-being, lifestyle behaviors, socio-demographic characteristics, and depression-related symptoms.

It was developed to support research in:

- Mental health analytics
- Psychosocial and behavioral research
- Depression-related risk assessment
- Supervised machine learning
- Explainable Artificial Intelligence (XAI)

The repository also includes a Jupyter Notebook documenting the data preprocessing, machine learning evaluation, and explainability workflow.

## 🎯 Research Objectives

The primary objectives of this dataset are to:

1. Investigate psychosocial and behavioral factors associated with depression-related symptoms.
2. Explore the relationships between lifestyle patterns and mental well-being.
3. Support the development of machine learning models for depression-related risk assessment.
4. Examine the contribution of individual features using explainable AI techniques.
5. Provide reusable survey data for mental health research in Bangladesh.

## 📊 Dataset at a Glance

| Attribute | Description |
|---|---|
| Total responses | 507 |
| Raw survey variables | 20 |
| Geographical coverage | Sylhet and Rajshahi, Bangladesh |
| Collection period | May–June 2026 |
| Data collection method | Self-administered survey |
| Questionnaire framework | DASS-21 depression subscale (adapted items) |
| Depression-related items | 7 |
| Derived variables | Depression_Score, Depression_Label |
| Data format | CSV |
| Analysis format | Jupyter Notebook |

## 🗂️ Repository Structure

```text
Bangladesh-Psychosocial-Health-Dataset/
│
├── Survey_Responses_Brief.csv
│
├── Ex_Mental(1).ipynb
│
└── README.md
```

| File | Description |
|---|---|
| `Survey_Responses_Brief.csv` | Structured survey dataset containing 507 responses. |
| `Ex_Mental.ipynb` | Jupyter Notebook containing preprocessing, machine learning, evaluation, and explainability analysis. |
| `README.md` | Documentation of the dataset and research methodology. |

## 🧩 Dataset Composition

The dataset covers four major conceptual domains.

### 1. Socio-demographic Characteristics

- Age
- Gender
- Highest education level
- Current occupation
- Marital status

### 2. Lifestyle and Behavioral Indicators

- Overall life satisfaction
- Sleep quality
- Daily screen time
- Physical activity frequency
- Social interaction frequency
- Academic/work-related stress

### 3. Mental Health History

- Self-reported prior mental health diagnosis

### 4. Depression-Related Symptoms

Seven symptom items adapted from the depression subscale of DASS-21:

- Sadness
- Worthlessness
- Anhedonia
- Hopelessness
- Meaninglessness
- Apathy
- Lack of initiative

Each item is rated on a four-point frequency scale ranging from **0 to 3**.

## 🧮 Derived Variables

Two additional variables are provided for quantitative and machine learning analysis.

| Variable | Description | Range |
|---|---|---|
| `Depression_Score` | Sum of the seven depression-related symptom items | 0–21 |
| `Depression_Label` | Binary classification target | 0 or 1 |

**Classification rule:**

- `0` = Non-depressed (Depression_Score below 10)
- `1` = Depressed (Depression_Score greater than or equal to 10)

These labels represent research-defined categories based on self-reported responses, not clinical diagnoses.

## 🤖 Machine Learning and Explainable AI

To demonstrate the dataset's suitability for supervised machine learning, ten classification algorithms were evaluated.

### Experimental Setup

- 80/20 stratified train–test split
- Ten classification algorithms
- Five-fold cross-validation
- Feature importance analysis
- SHAP-based explainability analysis

### Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Matthews Correlation Coefficient (MCC)
- Cohen's Kappa

### Reported Experimental Results

| Evaluation | Result |
|---|---:|
| Model accuracy range | 82.4%–98.0% |
| Majority-class baseline | 77.3% |
| Mean weighted F1-score (5-fold CV) | 0.840 |
| Cross-validation standard deviation | 0.062 |

These results demonstrate the dataset's potential for supervised learning experiments. They should not be interpreted as evidence of clinical diagnostic performance.

## 🔍 Explainability Analysis

SHAP (SHapley Additive exPlanations) is used to investigate how individual demographic, behavioral, and psychosocial features contribute to machine learning predictions.

The explainability analysis can help researchers:

- Identify influential predictive features.
- Understand individual model predictions.
- Examine relationships between behavioral indicators and depression-related outcomes.
- Improve the interpretability of machine learning models.

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/kushal15-neub/Bangladesh-Psychosocial-Health-Dataset.git
```

### 2. Navigate to the Project Directory

```bash
cd Bangladesh-Psychosocial-Health-Dataset
```

### 3. Install the Basic Requirements

```bash
pip install pandas numpy matplotlib seaborn scikit-learn shap jupyter
```

Additional dependencies may be required depending on the models and explainability methods implemented in the notebook.

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `Ex_Mental.ipynb` and follow the documented analysis workflow.

## 📖 Potential Research Applications

This dataset can be reused for:

- Depression-related symptom analysis.
- Psychosocial and behavioral factor investigation.
- Mental health data mining.
- Machine learning classification and regression.
- Feature selection and importance analysis.
- Explainable AI research.
- Comparative evaluation of predictive models.
- Public health and behavioral science research.

## Ethical Considerations and Limitations

This dataset contains self-reported survey responses manually collected over a period of approximately four months for academic research and educational purposes.

**Important considerations:**

- Participation was voluntary, and participants were informed about the purpose of the data collection before providing their responses.
- The shared dataset does not contain direct personal identifiers such as names, email addresses, telephone numbers, or residential addresses.
- The dataset does not contain clinically confirmed psychiatric diagnoses.
- The binary depression label was generated using a predefined research threshold and should not be interpreted as a clinical diagnosis.
- The seven depression-related symptom items were adapted from the DASS-21 depression subscale.
- The responses are self-reported and may be affected by response, recall, or interpretation bias.
- The dataset represents the population reached through the manual data-collection process and may therefore have sampling and regional representation limitations.
- Predictive outcomes generated using this dataset should not be used as substitutes for professional psychological or psychiatric assessments.
- The dataset is intended for academic research, educational purposes, and methodological experimentation and should not be used for clinical diagnosis or other high-stakes decisions about individuals.

## 📚 Citation

If you use this dataset in your research, please cite the following resource:

**Dataset title:** Bangladesh Psychosocial and Behavioral Health Survey Dataset

**Author:** Kushal Panthadas

**Repository:** GitHub

**Dataset DOI:** DOI:
10.17632/4s7dmcw5x7.1.

A suggested citation format:

Panthadas, K. (2026). *Bangladesh Psychosocial and Behavioral Health Survey Dataset*. Mendeley Data. https://doi.org/[DOI]

Please replace the DOI placeholder after the dataset receives its permanent DOI.

## 🤝 Contributions

Researchers interested in extending this dataset, conducting comparative experiments, or exploring additional explainable AI approaches are welcome to use this resource in accordance with applicable research ethics and data-sharing conditions.

## 👨‍💻 Author

**Kushal Panthadas**

B.Sc. in Computer Science and Engineering

North East University Bangladesh

Research Interests:

- Explainable Artificial Intelligence
- Machine Learning
- Mental Health Analytics
- Data Science
- Psychosocial and Behavioral Research

[GitHub](https://github.com/kushal15-neub) | [LinkedIn](https://linkedin.com/in/kushalpanthadas/)

---

<p align="center">

**Advancing Mental Health Research Through Data and Explainable AI 🇧🇩**

*Making psychosocial research data more accessible, reusable, and interpretable.*

</p>
