# MLBench — Multi-Modal Machine Learning Benchmark

A comparative machine learning project exploring different algorithms across numerical, image, and text data. The project covers the complete machine learning workflow, from data exploration and preprocessing to model training, hyperparameter tuning, evaluation, and deployment through a simple graphical user interface.

## Overview

MLBench aims to explore how different machine learning algorithms perform on different types of data and understand the strengths, limitations, and behavior of each model.

The project consists of three machine learning tasks:

- **Numerical Data:** Regression to predict a continuous target value.
- **Image Data:** Image classification into multiple categories.
- **Text Data:** Text classification into different labels.

Each task includes data preprocessing, feature extraction where applicable, model training, hyperparameter tuning, evaluation on unseen test data, and comparison between models.

## Project Objectives

- Perform exploratory data analysis (EDA) on real-world datasets.
- Handle missing values, categorical variables, and data inconsistencies.
- Apply appropriate preprocessing techniques for numerical, image, and text data.
- Extract meaningful features from images and text.
- Train and compare different machine learning algorithms.
- Tune model hyperparameters using validation data.
- Evaluate models using appropriate performance metrics.
- Apply unsupervised learning using K-Means clustering.
- Save trained models and use them to make predictions on new inputs.
- Develop a simple GUI to interact with the trained models.

## Project Parts

### Part A — Numerical Data (Regression)

Predict a continuous numerical value using two regression algorithms.

**Models:**
- Linear Regression
- K-Nearest Neighbors (KNN) Regressor

**Workflow:**
- Exploratory Data Analysis
- Data cleaning and missing-value handling
- Encoding categorical features
- Feature scaling
- Training, validation, and test splitting
- Hyperparameter tuning
- Model evaluation and comparison

**Evaluation Metrics:**
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score
- Predicted vs. Actual plots

### Part B — Image Data (Classification)

Classify images into 3–5 categories using supervised and unsupervised learning.

**Models:**
- Logistic Regression
- K-Nearest Neighbors (KNN) Classifier
- K-Means Clustering (unsupervised learning)

**Workflow:**
- Image exploration
- Image resizing
- Pixel normalization
- Feature extraction
- Training and validation
- Hyperparameter tuning
- K-Means clustering and cluster-to-label mapping
- Model evaluation and comparison

**Evaluation Metrics:**
- Accuracy
- Confusion Matrix
- Precision
- Recall
- F1-score
- Silhouette Score (for K-Means)

### Part C — Text Data (Classification)

Classify text samples into their corresponding categories using text-processing and machine learning techniques.

**Models:**
- Logistic Regression
- Linear Support Vector Machine (Linear SVM)

**Workflow:**
- Text cleaning and normalization
- Lowercasing
- Removing punctuation, numbers, stopwords, and HTML tags when applicable
- Feature extraction using Bag of Words or TF-IDF
- Training, validation, and test splitting
- Hyperparameter tuning
- Model evaluation and comparison

**Evaluation Metrics:**
- Accuracy
- Confusion Matrix
- Precision
- Recall
- F1-score per class

## GUI

The project includes a simple graphical user interface that allows users to interact with the trained models.

The application provides:

- Numerical input for regression predictions.
- Image upload for image classification.
- Text input for text classification.

The GUI loads previously trained and saved models without retraining them.

## Repository Structure

```text
MLBench/
├── datasets/
│   ├── numerical/
│   ├── images/
│   └── text/
│
├── part_a_numerical/
│   ├── notebooks/
│   ├── src/
│   └── results/
│
├── part_b_images/
│   ├── notebooks/
│   ├── src/
│   └── results/
│
├── part_c_text/
│   ├── notebooks/
│   ├── src/
│   └── results/
│
├── models/
│   ├── numerical/
│   ├── images/
│   └── text/
│
├── gui/
│   ├── app.py
│   └── pages/
│
├── report/
├── docs/
├── requirements.txt
└── README.md
```

## Technologies Used

- **Python**
- **NumPy** — Numerical computations
- **Pandas** — Data manipulation and analysis
- **Matplotlib & Seaborn** — Data visualization
- **Scikit-learn** — Machine learning algorithms, preprocessing, and evaluation
- **OpenCV / Pillow** — Image preprocessing
- **NLTK** — Text preprocessing
- **Streamlit / Gradio / Tkinter** — GUI development
- **Jupyter Notebook** — Experimentation and analysis
- **Git & GitHub** — Version control and collaboration

## Methodology

For each dataset, the following workflow is followed:

1. Explore and understand the raw dataset.
2. Perform data cleaning and preprocessing.
3. Split the data into training, validation, and test sets.
4. Extract or transform features when needed.
5. Train the required models.
6. Tune hyperparameters using validation data.
7. Evaluate the final models on the test set.
8. Compare model performance and analyze errors.
9. Save the trained models.
10. Integrate the models into the GUI.

All data splits use fixed random seeds to ensure reproducibility. The test set is kept separate during model selection and is used for final evaluation only.

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/MLBench.git
cd MLBench
```

Install the required packages:

```bash
pip install -r requirements.txt
```

## Running the Project

### Notebooks

Navigate to the notebook directory of the part you want to explore and run the notebooks in order.

### GUI

After training and saving the models, launch the application using:

```bash
streamlit run gui/app.py
```

> The GUI uses the saved models and preprocessing objects. Training is performed separately in the notebooks or training scripts.

## Results

The results section will contain the performance evaluation and comparison of the trained models across all three tasks.

| Task | Models | Evaluation |
|---|---|---|
| Numerical Regression | Linear Regression, KNN Regressor | MAE, RMSE, R² |
| Image Classification | Logistic Regression, KNN Classifier | Accuracy, Precision, Recall, F1, Confusion Matrix |
| Image Clustering | K-Means | Silhouette Score, Cluster-to-Label Mapping |
| Text Classification | Logistic Regression, Linear SVM | Accuracy, Precision, Recall, F1, Confusion Matrix |

Detailed results, visualizations, and discussion will be added as the project progresses.

## Team Contributions

Each team member contributes to different stages of the project, including preprocessing, feature extraction, model implementation, tuning, evaluation, GUI development, documentation, and testing.

Individual contributions will be documented in the final project report.

## Academic Integrity

All implementations, experiments, preprocessing pipelines, and analysis are developed and understood by the team members. Official documentation and course materials are used as references.

Every team member is expected to understand the methodology and implementation of all project parts.

---

**Course Project — Machine Learning**  
Academic Year 2026–2027
