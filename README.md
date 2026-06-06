# Data Structures and Algorithms

A comprehensive repository featuring practical applications of data structures, algorithms, and machine learning techniques. This project demonstrates key concepts through real-world data analysis, customer segmentation, and time series forecasting.

## Overview

This repository contains implementations and applications of fundamental computer science concepts including:
- **Data Analysis & Visualization**: Exploratory data analysis using Python's scientific stack
- **Machine Learning**: Regression models, clustering, and classification algorithms
- **Time Series Forecasting**: ARIMA models for predictive analytics
- **Data Processing**: Working with real-world datasets (Customer Loyalty Card Data, Walmart data)

Perfect for learning and demonstrating practical applications of data science and machine learning.


## Main Projects

### 1. Walmart Customer Analysis
**File**: `walmart_customer_analysis..py`

Comprehensive exploratory data analysis of customer loyalty card data.

**Features**:
- Display and explore dataset structure
- Basic statistical summary
- Gender distribution analysis
- Age distribution visualization
- Annual income analysis
- Spending score distribution

**Libraries Used**: `pandas`, `seaborn`, `matplotlib`

**Output**:
- Statistical summaries
- Count plots for categorical data
- Histograms for numerical distributions

**Example Usage**:
```bash
python walmart_customer_analysis..py
```

---

### 2. Customer Segmentation - K-Means Clustering
**File**: `customer_segmentation_K-Means_Clustering.py`

Unsupervised machine learning approach to segment customers into distinct groups.

**Features**:
- K-Means clustering algorithm implementation
- Elbow method for optimal cluster selection
- Cluster centers identification
- Cluster label assignment
- Visualization of customer segments

**Libraries Used**: `pandas`, `scikit-learn`, `matplotlib`

**Key Metrics**:
- Within-Cluster Sum of Squares (WCSS)
- Cluster centers
- Cluster labels

**Algorithm Details**:
```
1. Load customer data
2. Select features: Annual Income, Spending Score
3. Apply K-Means with k=4 clusters
4. Use Elbow Method to find optimal k (1-10)
5. Visualize clusters in 2D space
```

**Example Usage**:
```bash
python customer_segmentation_K-Means_Clustering.py
```

**Output**:
- Cluster centers
- Elbow graph for optimal cluster determination
- 2D scatter plot with color-coded clusters

---

### 3. Data Analysis with Regression and ARIMA
**File**: `DataAnalysisWithRegression_and_arima.py`

Advanced time series and predictive modeling combining regression and forecasting techniques.

**Features**:

**A. Linear Regression**
- Supervised learning for continuous prediction
- Train-test split (80-20)
- Data standardization/scaling
- Coefficient and intercept analysis
- Scatter plot: Original vs. Predicted values

**B. Logistic Regression**
- Classification algorithm
- Multi-class classification support
- Confusion matrix generation
- Model performance visualization

**C. ARIMA (AutoRegressive Integrated Moving Average)**
- Time series forecasting
- ARIMA(1,1,1) model configuration
- 10-step ahead forecasting
- Original vs. forecasted values visualization

**Libraries Used**: `pandas`, `scikit-learn`, `statsmodels`, `matplotlib`, `seaborn`, `numpy`

**Process**:
```
1. Load CustomerLoyaltyCardData.csv
2. Data preparation and feature engineering
3. Train-test split with scaling
4. Fit Linear Regression model
5. Fit Logistic Regression model
6. Generate ARIMA forecast
7. Visualize results with multiple plots
```

**Example Usage**:
```bash
python DataAnalysisWithRegression_and_arima.py
```

**Output**:
- Linear regression coefficients and intercept
- Scatter plot comparison
- Logistic regression confusion matrix heatmap
- ARIMA forecast values
- Time series plot with forecasted trend

---

## Dataset

### CustomerLoyaltyCardData.csv
Customer shopping and demographic data used across all projects.

**Features**:
- **CustomerID**: Unique identifier
- **Gender**: Customer gender (M/F)
- **Age**: Customer age
- **Annual Income (k$)**: Annual income in thousands of dollars
- **Spending Score (1-100)**: Spending behavior score

**Size**: 3,780 bytes
**Records**: ~200-500 customer entries

---

## Installation & Setup

### Prerequisites
- Python 3.7+
- pip (Python package manager)

### Required Libraries

```bash
pip install pandas scikit-learn statsmodels matplotlib seaborn numpy
```

### Or using requirements file

Create `requirements.txt`:
```
pandas>=1.3.0
scikit-learn>=0.24.0
statsmodels>=0.13.0
matplotlib>=3.4.0
seaborn>=0.11.0
numpy>=1.21.0
```

Install all dependencies:
```bash
pip install -r requirements.txt
```

### Virtual Environment Setup (Recommended)

```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Linux/Mac:
source venv/bin/activate
# On Windows:
venv\Scripts\activate

# Install dependencies
pip install pandas scikit-learn statsmodels matplotlib seaborn numpy
```

---

## Usage Examples

### Run All Projects
```bash
# Make sure you're in the repository directory
python walmart_customer_analysis..py
python customer_segmentation_K-Means_Clustering.py
python DataAnalysisWithRegression_and_arima.py
```

### Individual Project Analysis

**Analyze customer demographics:**
```bash
python walmart_customer_analysis..py
```
Expected output: Visualizations of gender, age, income, and spending distributions

**Identify customer segments:**
```bash
python customer_segmentation_K-Means_Clustering.py
```
Expected output: Elbow curve, optimal cluster visualization, and cluster assignments

**Predict and forecast:**
```bash
python DataAnalysisWithRegression_and_arima.py
```
Expected output: Regression performance metrics, confusion matrix, and time series forecast

---

## Machine Learning Algorithms Explained

### K-Means Clustering
**Purpose**: Unsupervised learning to group customers into k clusters

**Algorithm**:
1. Initialize k random centroids
2. Assign each point to nearest centroid
3. Calculate new centroids based on cluster members
4. Repeat until convergence

**Use Case**: Customer segmentation for targeted marketing

### Linear Regression
**Purpose**: Predict continuous values based on input features

**Formula**: `y = mx + b`

**Use Case**: Predicting customer spending based on demographics

### Logistic Regression
**Purpose**: Binary/multi-class classification

**Use Case**: Classifying customer behavior patterns

### ARIMA(p,d,q)
**Purpose**: Time series forecasting

**Parameters**:
- **p**: AutoRegressive order
- **d**: Differencing order (for stationarity)
- **q**: Moving Average order

**Use Case**: Predicting future spending trends

---

## Key Concepts & Skills Demonstrated

### Data Science Fundamentals
- ✅ Data loading and exploration
- ✅ Feature engineering and selection
- ✅ Data preprocessing and scaling
- ✅ Train-test data splitting
- ✅ Model evaluation and validation

### Machine Learning
- ✅ Supervised learning (Regression, Classification)
- ✅ Unsupervised learning (Clustering)
- ✅ Model fitting and prediction
- ✅ Hyperparameter tuning (Elbow method)

### Data Visualization
- ✅ Scatter plots
- ✅ Histograms
- ✅ Count plots
- ✅ Heatmaps (Confusion matrices)
- ✅ Time series plots

### Statistics & Analytics
- ✅ Descriptive statistics
- ✅ Distribution analysis
- ✅ Correlation analysis
- ✅ Forecasting

---

## Performance Metrics & Results

### K-Means Clustering
- **Optimal Clusters**: 4 (determined by Elbow method)
- **Features Used**: Annual Income, Spending Score
- **WCSS Range**: Varies based on k value (1-10)

### Regression Models
- **Train-Test Split**: 80-20
- **Scaling Method**: StandardScaler
- **Test Size**: 20% of data

### ARIMA Forecast
- **Model**: ARIMA(1,1,1)
- **Forecast Horizon**: 10 steps
- **Data Source**: Customer Age

---

## Educational Value

This repository is excellent for learning:

### For Beginners
- Python data manipulation with Pandas
- Data visualization with Matplotlib and Seaborn
- Basic machine learning concepts
- Working with CSV datasets

### For Intermediate Learners
- Scikit-learn model implementation
- Multiple algorithm comparison
- Cluster analysis and interpretation
- Time series analysis with ARIMA

### For Advanced Users
- Real-world data science workflows
- Model evaluation strategies
- Business analytics applications
- Predictive modeling pipelines

---

## Potential Enhancements

Future improvements could include:
- [ ] Cross-validation for model robustness
- [ ] Feature importance analysis
- [ ] GridSearchCV for hyperparameter optimization
- [ ] Additional clustering algorithms (DBSCAN, Hierarchical)
- [ ] Advanced ARIMA diagnostics
- [ ] Deep learning models (Neural Networks)
- [ ] Dashboard/web interface
- [ ] Real-time data processing
- [ ] A/B testing framework

---

## Common Issues & Solutions

### Issue: "Module not found" error
**Solution**: Install missing packages
```bash
pip install pandas scikit-learn statsmodels matplotlib seaborn
```

### Issue: CSV file not found
**Solution**: Ensure `CustomerLoyaltyCardData.csv` is in the same directory as scripts

### Issue: Warning messages during execution
**Solution**: Already handled with `warnings.filterwarnings("ignore")` in scripts

### Issue: Plot windows not displaying
**Solution**: Add `plt.show()` is called; may need to configure matplotlib backend

---

## License

This project is licensed under the **Apache License 2.0** - see the [LICENSE](LICENSE) file for details.

```
Copyright 2022 CodeDroid999.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0
```

---

## Author

**CodeDroid999**

---

## Contributing

Contributions are welcome! Feel free to:
- Report bugs and issues
- Suggest improvements and enhancements
- Submit pull requests with new features
- Add additional algorithms and techniques

---

## References

### Libraries & Documentation
- [Pandas Documentation](https://pandas.pydata.org/)
- [Scikit-Learn Documentation](https://scikit-learn.org/)
- [Statsmodels Documentation](https://www.statsmodels.org/)
- [Matplotlib Documentation](https://matplotlib.org/)
- [Seaborn Documentation](https://seaborn.pydata.org/)

### Machine Learning Resources
- [K-Means Clustering](https://en.wikipedia.org/wiki/K-means_clustering)
- [Linear Regression](https://en.wikipedia.org/wiki/Linear_regression)
- [Logistic Regression](https://en.wikipedia.org/wiki/Logistic_regression)
- [ARIMA Models](https://en.wikipedia.org/wiki/Autoregressive_integrated_moving_average)

---

## Repository Stats

- **Language**: Python
- **Size**: ~114 KB
- **Last Updated**: May 2026
- **Stars**: 4
- **License**: Apache 2.0

---

**Happy Learning & Coding! 🚀**
