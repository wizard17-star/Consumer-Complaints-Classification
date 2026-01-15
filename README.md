# Consumer Complaints Classification Project

Real CFPB Consumer Complaints dataset using text-based machine learning with advanced optimization.

## 📊 Project Overview

- **Data**: 277,814 real complaints → **10,000 samples** (stratified)
- **Classes**: Top 5 product categories (3.36:1 imbalance)
- **Best Model**: Logistic Regression + SMOTE
- **Performance**: F1=**0.7465** (74.65%) | **+2.49%** improvement
- **Author**: Serhat Aslan (s34090)

---

## 📁 Project Structure

```
Wum Project/
├── notebooks/
│   └── complete_analysis.ipynb           # Full pipeline (22 cells)
│
├── results/
│   ├── 04_model_comparison_4models.png    # 4-model comparison
│   ├── learning_curves.png                # Training dynamics
│   ├── confusion_matrix.png               # Test set matrix
│   └── 05_optimization_comparison.png     # Optimization results
│
├── presentation.md                       # Markdown presentation
├── presentation.html                     # Web-viewable presentation
├── final_results.md                      # Complete analysis
├── quickstart.md                         # Setup & run guide
├── README.md                             # This file
├── requirements.txt                      # Dependencies
└── .gitignore                            # Git ignore file
```

---

## ✅ What's Included

### Analysis & Models
✅ **Data Processing**: 277K → 10K balanced dataset  
✅ **Feature Engineering**: 5,000 TF-IDF features  
✅ **4-Model Comparison**: SVM, LogReg, RandomForest, NaiveBayes  
✅ **Hyperparameter Tuning**: Optimal C values identified  
✅ **Advanced Optimization**:
  - GridSearchCV (F1=0.734, +0.80%)
  - Voting Classifier (F1=0.744, +2.14%)
  - **SMOTE (F1=0.747, +2.49%)** 🏆

### Results
✅ **Best Model**: LogReg + SMOTE  
✅ **Precision**: 0.7393  
✅ **Recall**: 0.7561  
✅ **F1-Score**: **0.7465** (74.65%)

---

## � Dataset Download

The dataset file (`data/Consumer_Complaints.csv`, ~515 MB) is **not included** in the repository due to file size limitations.

**Download the dataset:**
1. Go to: [Kaggle - Consumer Complaints Dataset](https://www.kaggle.com/datasets/dushyantv/consumer_complaints?resource=download)
2. Download `Consumer_Complaints.csv`
3. Place it in the `data/` folder: `Wum Project/data/Consumer_Complaints.csv`

---

## 🚀 Quick Start

### 1. Download Dataset
- Follow the instructions above to get `Consumer_Complaints.csv`

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Run Full Analysis
```bash
cd notebooks
jupyter notebook complete_analysis.ipynb
# Run all cells - takes ~5 minutes
```

### 4. View Results
- **Presentation**: Open `presentation.html`
- **Detailed Results**: Read `final_results.md`
- **Quick Reference**: See `quickstart.md`

---

## 📊 Key Results

### 4-Model Comparison
| Model | F1-Score |
|-------|----------|
| Linear SVM | 0.7500 ⭐ |
| Logistic Regression | 0.7416 |
| Random Forest | 0.7186 |
| Naive Bayes | 0.6060 |

### Optimization Results
| Technique | F1-Score | Improvement |
|-----------|----------|------------|
| **LogReg + SMOTE** 🏆 | **0.7465** | **+2.49%** |
| Voting Classifier | 0.7439 | +2.14% |
| GridSearchCV | 0.7341 | +0.80% |
| Baseline SVM | 0.7283 | - |

### Per-Class Performance
| Category | F1 |
|----------|-----|
| Mortgage | 0.92 |
| Debt Collection | 0.86 |
| Credit Card | 0.79 |
| Credit Repair | 0.66 |
| Credit Reporting | 0.53 |

---

## 💡 Key Insights

**Strengths**:
- ✅ Realistic metrics (74.65%, not overfitted)
- ✅ Balanced predictions (Precision ≈ Recall)
- ✅ Handles 3.36:1 class imbalance well
- ✅ Stable generalization (Val → Test)

**Challenges**:
- ⚠️ Semantic similarity in categories
- ⚠️ Text overlap across classes
- ⚠️ Minority classes harder to predict
- ⚠️ TF-IDF loses word context

---

## 📖 Documentation Files

- **FINAL_RESULTS.md** - Complete analysis, detailed metrics, all findings
- **QUICKSTART.md** - Setup instructions, how to run, key files
- **README.md** - This file, project overview

---

## 🎯 Status

✅ **COMPLETE** - All analysis done, models optimized, presentations ready  
✅ **COMPLETE** - Full analysis and evaluation done  
✅ **DOCUMENTED** - Full results and insights included

---

**Author**: Serhat Aslan (s34090)  
**Date**: January 15, 2026  
**Best Model**: Logistic Regression + SMOTE  
**Final F1-Score**: 0.7465
