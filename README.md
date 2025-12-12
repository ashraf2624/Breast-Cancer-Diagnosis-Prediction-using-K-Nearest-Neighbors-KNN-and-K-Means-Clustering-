# Breast-Cancer-Diagnosis-Prediction-using-K-Nearest-Neighbors-KNN-and-K-Means-Clustering-
This project uses machine learning techniques to classify breast cancer tumors as Benign (B) or Malignant (M) based on diagnostic measurements from the Breast Cancer Wisconsin dataset.

This project performs:

Data Cleaning
1.Encoding (M → 1, B → 0)
2.Dropping unused columns (id, Unnamed: 32)
3.Min-Max Normalization
4.K-Means Clustering (k = 2)
5.Train-Test Split (80/20)
6.KNN Classification (k = 5)
7.Model Evaluation (Accuracy, Precision, Recall, F1-score)
Both unsupervised and supervised techniques are used to understand and classify cancer data.

Preprocessing Steps:

1. Encode Diagnosis
Converted the diagnosis column using LabelEncoder or mapping:
M = 1 (Malignant)
B = 0 (Benign)

2. Drop Unnecessary Columns
id
Unnamed: 32

3. Feature Scaling
Min-Max Scaler was applied to normalize all feature values between 0 and 1.

4. Train-Test Split
The dataset was split into:
80% Training
20% Testing

Machine Learning Models Used
1. K-Means Clustering (k = 2)
K-Means is used as an unsupervised technique to see how well the dataset naturally separates into two groups (benign vs malignant).
The clustering results do not always match exact labels, because:
K-Means does not know the diagnosis labels
Cluster numbers (0/1) do not represent benign/malignant
Some samples overlap in feature space
This step helps visualize natural grouping in data.

2. KNN Classifier (k = 5)

KNN is used as the main supervised classification model.
KNN was trained using the 80% training data
Predictions were made on the test set
Evaluation metrics were calculated

Evaluation Metrics

After training the KNN classifier, the following metrics were computed:
1.Accuracy
2.Precision
3.Recall
4.F1-score

These metrics help assess the model’s performance in detecting malignant tumors.

