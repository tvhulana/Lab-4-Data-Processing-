Lab 4: Data Preprocessing Techniques

1. Handling Missing Data

Identify missing values with isnull().

Remove rows/columns with dropna().

Impute missing values with SimpleImputer (mean, median, most_frequent).


2. Handling Categorical Data

Ordinal features: Encode with custom mappings (e.g., size → S=0, M=1, L=2).

Nominal features: Encode using One-Hot Encoding (OneHotEncoder, pd.get_dummies).

Class labels: Encode with LabelEncoder.



3. Partitioning Dataset

Split dataset into train/test with train_test_split().

Use stratify=y to keep class proportions balanced.


4. Feature Scaling

Normalization (MinMaxScaler): Scales features between 0 and 1.

Standardization (StandardScaler): Mean = 0, Std = 1.


5. Feature Selection

L1 Regularization (Lasso): Shrinks less important features’ coefficients to zero.

SBS (Sequential Backward Selection): Iteratively removes least useful features.

Random Forest Feature Importance: Ranks features by contribution.




Questions & Reflections

Why is handling missing data important?
 Because ML algorithms cannot work with NaNs. Missing data may bias results.

When use One-Hot vs Label Encoding?
 Label encoding = ordinal features, One-hot = nominal features.

How does scaling impact KNN or SVM?
Prevents large-range features from dominating distance calculations.

Compare L1 vs SBS?

 L1 = automatic & efficient, SBS = interpretable but slower.
