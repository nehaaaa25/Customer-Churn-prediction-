# Customer-Churn-prediction-
Here we analyse datas, and see whether a customer gets churned or not 
Programming and tools

Python
Google Colab / Jupyter notebooks (including uploading files with google.colab.files)
Libraries: pandas, NumPy, Matplotlib, Seaborn, SciPy, scikit-learn

Data handling and cleaning

Loading and inspecting CSV data (head, info, describe, nunique)
Finding and removing duplicate rows
Measuring missing values, then filling them: median for numbers, mode for categories
Spotting invalid data (a negative income value) and fixing it
Checking for outliers with the IQR method, and deciding not to cap values that were real
Checking category values for inconsistent spellings

Exploratory data analysis (EDA) and statistics

Descriptive statistics: mean, median, variance, skewness
Histograms, boxplots, density plots, count plots, pair plots, bar charts
Correlation analysis: Pearson, Spearman, Kendall, and a correlation heatmap
Cramér’s V with a chi-square test, for how categories relate to churn
Churn rate broken down by each category
Checking whether the two classes are balanced

Feature engineering and preprocessing

One-hot encoding, with a stated reason for choosing it over label encoding
Building new interaction features: ratios, tenure measures, flag features
Feature selection with Random Forest feature importance and Mutual Information
Feature scaling with StandardScaler and MinMaxScaler
A stratified train/test split, with the scaler fitted on training data only so test data doesn’t leak in

Machine learning: supervised

Logistic Regression
Decision Tree (depth limited to reduce overfitting)
Random Forest (an ensemble of trees)
Neural Network (MLPClassifier with early stopping)

Machine learning: unsupervised

K-Means clustering
Choosing k with the elbow method and silhouette score
Mapping clusters to the real churn labels by majority vote
PCA to reduce the data to 2 dimensions for plotting

Model evaluation

Confusion matrices
Accuracy, Precision, Recall, F1-score, classification reports
ROC curves and AUC
Clustering metrics: Silhouette score, Adjusted Rand Index, Normalized Mutual Information
Comparing all models side by side against a random-guess baseline

Analysis and communication

Explaining each result in markdown notes
Reporting negative results honestly (the features carry almost no signal)
Writing up limitations and future work, such as XGBoost, GridSearchCV, and SMOTE
