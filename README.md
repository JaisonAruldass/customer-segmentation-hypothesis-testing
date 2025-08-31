🎯 Project Overview
This project demonstrates professional-grade customer analytics by applying advanced statistical methods to understand mall customer behavior patterns. Unlike typical customer analysis projects, this implementation emphasizes statistical rigor, proper validation, and business-actionable insights.
Key Differentiators

✅ Proper Statistical Testing with assumption validation
✅ Multiple Testing Correction (FDR method)
✅ Effect Size Reporting for practical significance
✅ Robust Clustering Validation with stability analysis
✅ Cross-Validated Predictive Models
✅ Business-Focused Feature Engineering

📊 Dataset
The analysis uses mall customer data containing:

Demographics: Age, Gender
Financial: Annual Income (k$)
Behavioral: Spending Score (1-100)
Sample Size: 200 customers

🔬 Methodology
Statistical Analysis Pipeline
1. Data Quality Assessment

Missing value detection
Outlier identification (IQR method)
Data type validation
Range verification

2. Feature Engineering with Business Logic
python# Created Features:
Life_Stage          # Young_Adult, Early_Career, Mid_Career, Mature
Income_Level        # Low, Medium, High (based on terciles)
Spending_Level      # Conservative, Moderate, High_Spender
Spending_Efficiency # Spending relative to income capacity
Age_Adjusted_Spending # Lifecycle-normalized spending patterns
3. Hypothesis Testing Framework
HypothesisStatistical TestPurposeGender → SpendingWelch's t-test / Mann-Whitney UTest gender differencesLife Stage → SpendingOne-way ANOVA / Kruskal-WallisTest age group differencesCombined EffectsTwo-way ANOVATest interaction effectsIncome ↔ SpendingChi-square testTest categorical associations
4. Advanced Clustering Analysis

Algorithm: K-means with standardized features
Optimization: Elbow method + Silhouette analysis
Validation: 10-fold stability analysis through resampling
Quality Metrics: Silhouette scores, inertia tracking

5. Predictive Modeling

Classification: Random Forest → Predict spending categories
Regression: Random Forest → Predict exact spending scores
Validation: Stratified K-fold cross-validation
Feature Importance: Identify key behavioral drivers

📈 Key Results
Statistical Findings

Multiple Testing Correction Applied: FDR (Benjamini-Hochberg) method
Effect Sizes Reported: Small, medium, large classifications
Assumption Validation: Normality and homogeneity tests performed

Customer Segmentation

Optimal Clusters: Determined via silhouette analysis
Stability Validated: Through resampling techniques
Business Profiles: Each segment mapped to marketing strategies

Predictive Performance

Classification: Cross-validated accuracy with confidence intervals
Regression: RMSE and R² on held-out test set
Feature Rankings: Most important predictors identified
