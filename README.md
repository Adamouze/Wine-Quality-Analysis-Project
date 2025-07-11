# Wine Quality Analysis Project

A comprehensive data analysis project focused on wine quality prediction using physicochemical properties of Portuguese wines.

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Key Analyses](#key-analyses)
- [Machine Learning Models](#machine-learning-models)
- [Results](#results)
- [Authors](#authors)

## 🍷 Project Overview

This project analyzes the quality of Portuguese wines (both red and white) based on their physicochemical properties. The main objectives are:

- Exploratory data analysis of wine characteristics
- Statistical analysis and correlation studies
- Principal Component Analysis (PCA) for dimensionality reduction
- Machine learning models for wine quality prediction
- Comparative analysis between red and white wines

## 📊 Dataset

The project uses two datasets from the UCI Machine Learning Repository:

- **Red Wine Dataset**: 1,599 samples with 11 physicochemical features
- **White Wine Dataset**: 4,898 samples with 11 physicochemical features

### Features analyzed:
- Fixed acidity
- Volatile acidity
- Citric acid
- Residual sugar
- Chlorides
- Free sulfur dioxide
- Total sulfur dioxide
- Density
- pH
- Sulphates
- Alcohol
- **Quality** (target variable, score 0-10)

**Combined Dataset**: 6,497 wine samples total

## 📁 Project Structure
├── wine+quality/ 
│ ├── winequality-red.csv # Red wine dataset 
│ ├── winequality-white.csv # White wine dataset 
│ └── winequality.names # Dataset description 
├── Rapport Etude Préliminaire - Projet AD 2023 - Adam Ouzegdouh - Kamil MAZAN.ipynb 
├── Rapport du Projet d'Analyse de Données - Analyse de la qualité des vins - Adam Ouzegdouh - Kamil MAZAN.pdf 
└── Projet_FIPA_AD.pdf

## 🔍 Key Analyses

### 1. Exploratory Data Analysis
- **Data Quality Assessment**: [View in notebook](Rapport%20Etude%20Préliminaire%20-%20%20Projet%20AD%202023%20-%20Adam%20Ouzegdouh%20-%20Kamil%20MAZAN.ipynb)
  - Missing values analysis
  - Data types verification
  - Outlier detection using IQR method

### 2. Statistical Analysis
- **Descriptive Statistics**: Comprehensive statistical summary of all variables
- **Quality Comparison**: 
  - Red wine average quality: 5.64
  - White wine average quality: 5.88
  - Difference: ~4.1%

### 3. Correlation Analysis
- **Correlation Matrix**: Analysis of relationships between physicochemical properties
- **Quality Correlations**: Identification of features most correlated with wine quality
- **Key Finding**: Alcohol content shows the strongest positive correlation with quality

### 4. Variance Analysis
- **Feature Variability**: Assessment of variance across all features
- **Distribution Analysis**: Box plots showing quality distributions for each feature

### 5. Principal Component Analysis (PCA)
- **Dimensionality Reduction**: Standardized data transformation
- **Component Analysis**: Identification of principal components explaining data variance

## 🤖 Machine Learning Models

### Random Forest Classifier
- **Model Type**: Ensemble learning method for classification
- **Data Split**: 80% training, 20% testing
- **Features**: All physicochemical properties (excluding quality)
- **Target**: Wine quality scores

### Model Performance
- **Classification Report**: Detailed precision, recall, and F1-scores
- **Confusion Matrix**: Model prediction accuracy visualization
- **Feature Importance**: Analysis of most influential features for quality prediction

## 📈 Results

### Key Findings:
1. **Quality Distribution**: Most wines score between 5-7 on the quality scale
2. **Alcohol Impact**: Higher alcohol content correlates with better quality ratings
3. **Outlier Analysis**: Quality variable shows 228 outliers in the combined dataset
4. **Type Comparison**: White wines have slightly higher average quality than red wines
5. **Feature Relationships**: Strong correlations exist between certain physicochemical properties

### Outlier Summary:
- **Quality outliers**: 228 samples (wines with exceptional ratings)
- **Alcohol outliers**: 3 samples with extreme alcohol content
- **Other variables**: Various outlier counts across different features

## 👥 Authors

- **Adam Ouzegdouh**
- **Kamil Mazan**

## 📚 Additional Resources

- [Full Analysis Report (PDF)](Rapport%20du%20Projet%20d'Analyse%20de%20Données%20-%20Analyse%20de%20la%20qualité%20des%20vins%20-%20Adam%20Ouzegdouh%20-%20Kamil%20MAZAN.pdf)
- [Project Specifications](Projet_FIPA_AD.pdf)

*Project completed: January 5, 2024*

---