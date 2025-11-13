# Traffic Sign Recognition System


> Machine Learning portfolio project achieving 15% accuracy improvement on German Traffic Sign Benchmark through ensemble methods, dimensionality reduction, and advanced optimization techniques.

## Overview

This comprehensive ML system classifies German traffic signs using multiple machine learning algorithms with systematic optimization. The project demonstrates end-to-end ML pipeline development including data preprocessing, feature engineering, model training, hyperparameter tuning, and performance evaluation.

**Key Results:**
- 📈 **15% Classification Accuracy Improvement**
- 🎯 **25% Reduction in Feature Space** (via PCA)
- 📊 **25% Increase in Model Precision**
- ✅ **10% F1-Score Improvement**
- 🔧 **Bayesian Hyperparameter Optimization**

## Dataset

**German Traffic Sign Recognition Benchmark (Subset)**
- **Source**: Stallkamp et al. benchmark dataset
- **Size**: 9,690 grayscale images (48×48 pixels)
- **Classes**: 10 traffic sign categories
- **Features**: 2,304 pixel values per image (48×48 flattened)

**Traffic Sign Categories:**
| Class | Sign Type |
|-------|-----------|
| 0 | Speed Limit 20 |
| 1 | Speed Limit 30 |
| 2 | Speed Limit 50 |
| 3 | Speed Limit 60 |
| 4 | Speed Limit 70 |
| 5 | Left Turn |
| 6 | Right Turn |
| 7 | Beware Pedestrian Crossing |
| 8 | Beware Children |
| 9 | Beware Cycle Route Ahead |

**Dataset Characteristics:**
- Grayscale images with pixel values 0-255
- Uniform 48×48 resolution
- Captured under varying lighting conditions
- Different times of day
- Real-world street sign variability

## 🔬 Methodology

### 1. Data Preprocessing
- Pixel normalization (0-1 range)
- Feature standardization using StandardScaler
- Train-test split with stratification
- Class distribution analysis

### 2. Dimensionality Reduction
**Principal Component Analysis (PCA):**
- Reduced 2,304 features to optimal subset
- **25% reduction in feature space**
- Preserved 95% of variance
- Improved computational efficiency
- Reduced overfitting risk

### 3. Class Imbalance Handling
**SMOTE (Synthetic Minority Over-sampling Technique):**
- Balanced class distribution
- Generated synthetic training samples
- Improved minority class performance
- **25% precision increase**

### 4. Model Development

**Algorithms Implemented:**
- **Random Forest**: Ensemble of decision trees
- **Decision Trees**: Baseline comparison
- **Support Vector Machines (SVM)**: RBF and linear kernels
- **Neural Networks**: Multi-layer perceptron

### 5. Hyperparameter Optimization

**Bayesian Optimization:**
- Efficient search over hyperparameter space
- Reduced tuning time vs. grid search
- Optimized parameters:
  - Tree depth, number of estimators
  - Learning rates, regularization
  - SVM kernel parameters
  - Neural network architecture

## 📈 Model Performance

| Model | Baseline Accuracy | Optimized Accuracy | Improvement |
|-------|------------------|-------------------|-------------|
| **Random Forest** | 82.3% | **94.7%** | **+12.4%** |
| Neural Network | 78.5% | 92.1% | +13.6% |
| SVM (RBF) | 85.1% | 93.4% | +8.3% |
| Decision Tree | 76.2% | 88.9% | +12.7% |

**Best Model Performance:**
- **Algorithm**: Random Forest (optimized)
- **Accuracy**: 94.7%
- **Precision**: 94.2%
- **Recall**: 94.5%
- **F1-Score**: 94.3% (+10% over baseline)

## 📊 Optimization Results

**Impact of Individual Techniques:**
- PCA Dimensionality Reduction: +5% accuracy, -40% training time
- SMOTE Class Balancing: +8% minority class recall, +25% precision
- Bayesian Optimization: +7% overall accuracy
- Ensemble Methods: +15% vs. single Decision Tree

**Combined Pipeline Performance:**
- Total accuracy improvement: **15%**
- Reduced false positives: **15%**
- Balanced precision-recall trade-off
- 3x faster inference time (due to PCA)


---

**Author**: Cheryl Biju | [GitHub](https://github.com/cbm2001) | [LinkedIn](https://linkedin.com/in/cheryl-biju)
