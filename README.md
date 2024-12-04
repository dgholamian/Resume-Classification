# Resume Classification Using BERT and DistilBERT Models (Multi-class classification)

This project focuses on fine-tuning **BERT** and **DistilBERT**, transformer-based pre-trained language models, to classify a dataset of 2,400 resumes into 24 distinct categories. Key components of the implementation include:

- **Text Cleaning**: Utilized the `spaCy` library for efficient text preprocessing and cleaning.
- **Visualization**: Employed Word Clouds and bar plot to gain insights into the data distribution and key features.
- **Overfitting Mitigation**: Implemented the early stopping technique to prevent overfitting during training.
- **Validation Strategy**: Adopted a stratified hold-out approach to ensure balanced representation across categories during model evaluation.
- **Performance Metric**: As the dataset is roughly balanced, accuracy was selected as the primary performance metric.

## ![Usage Icon](https://img.shields.io/badge/Usage-blue) Usage

The `main.ipynb` file contains all the steps involved in this project. The notebook is organized into clearly defined sections, each representing a distinct step of the workflow:

1. **Data Preparation**: Loading and preprocessing the resume dataset using `spaCy` for text cleaning.
2. **Visualization**: Creating Word Clouds and bar plots to explore and understand the data.
3. **Model Fine-Tuning**: Fine-tuning `BERT` and `DistilBERT` classifiers for multi-category classification of resumes.
4. **Optimization**: Using the early stopping technique to prevent overfitting.
5. **Evaluation**: Employing a stratified hold-out approach to validate model performance and using accuracy as the primary metric.

Follow the notebook step by step to reproduce the results or adapt the workflow for similar datasets.


## ![Data Source Icon](https://img.shields.io/badge/Data%20Source-orange) Data Source

The dataset used in this project consists of 2,400 resumes originally in PDF format, converted into structured CSV data for easier processing. It includes:

- **Textual Content**: Extracted resume text for analysis and modeling.

This dataset serves as the foundation for building the classification model. It can be accessed via Kaggle at [this link](https://www.kaggle.com/datasets/snehaanbhawal/resume-dataset).

You will need a Kaggle account to download the dataset.


## ![Project Steps Icon](https://img.shields.io/badge/Project%20Steps-blue) Project Steps

This project is divided into the following key steps:

### 1. **Data Processing**
   - Preprocessing resume text using the `spaCy` library.
   - Converting PDF resumes into structured CSV format.

### 2. **Data Partitioning**
   - Splitting the dataset into training, validation, and test sets using a stratified hold-out approach.

### 3. **Model Definition**
   - Defining and fine-tuning transformer-based models (`BERT` and `DistilBERT`).

### 4. **Training BERT**
   - Fine-tuning `BERT` for resume classification into 24 categories.

### 5. **Training DistilBERT**
   - Fine-tuning `DistilBERT` as a lighter alternative to `BERT`.

### 6. **Evaluation**
   - Evaluating model performance using metrics such as accuracy and confusion matrices.

### 7. **Results**
   The following visualizations and metrics were generated during the project:

   #### 7.1. Word Cloud Before Cleaning Text
   - [Word Cloud Before Cleaning Text](#custom-id)
   - Visual representation of the text data before applying cleaning techniques.

   #### 7.2. **Word Cloud Before Cleaning Text Per Category**
   - Word cloud analysis for each resume category before text cleaning.

   #### 7.3. **Word Cloud After Cleaning Text**
   - Word cloud visualization after text cleaning to highlight meaningful features.

   #### 7.4. **Word Cloud After Cleaning Text Per Category**
   - Per-category word clouds generated after text cleaning.

   #### 7.5. **Bar Plot for Checking Label Distribution**
   - Visual representation of the distribution of labels across the dataset.

   #### 7.6. **BERT Accuracy (Training and Validation Dataset)**
   - Accuracy achieved by the `BERT` model on training and validation datasets.

   #### 7.7. **BERT Loss (Training Dataset)**
   - Loss trajectory during `BERT` training.

   #### 7.8. **DistilBERT Accuracy (Training and Validation Dataset)**
   - Accuracy achieved by the `DistilBERT` model on training and validation datasets.

   #### 7.9. **DistilBERT Loss (Training Dataset)**
   - Loss trajectory during `DistilBERT` training.

   #### 7.10. **BERT Confusion Matrix (Test Dataset)**
   - Confusion matrix for `BERT` predictions on the test dataset.

   #### 7.11. **DistilBERT Confusion Matrix (Test Dataset)**
   - Confusion matrix for `DistilBERT` predictions on the test dataset.

  
  
  
   <h4 id="custom-id">Word Cloud Before Cleaning Text</h4>
   ![Word Cloud Before Cleaning Text](https://github.com/dgholamian/Resume-Classification/blob/main/figures/word_cloud_raw_text.png)
