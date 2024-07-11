# Diabetes-Prediction-Model
This project is a ML model which aims to predict diabetes from a given dataset of people (Pima India). 
The objective of this project is to develop a machine learning model that can accurately predict diabetes based on various medical attributes. Early prediction of diabetes can significantly help individuals take necessary precautions and modify their lifestyle to manage or even prevent this chronic disease.

First, we import essential libraries such as Pandas for data manipulation, NumPy for numerical computations, Seaborn and Matplotlib for data visualization, and Scikit-learn for machine learning algorithms and evaluation metrics.

Next, we load the Pima Indians Diabetes Database from Kaggle. This dataset contains medical information for 768 individuals, including attributes like glucose levels, blood pressure, BMI, age, and diabetes pedigree function. We inspect the first few rows of the dataset to get an overview of the data structure.

Data preprocessing is a crucial step in any machine learning project. Here, we check for missing values and replace zeros in certain columns with NaN. We then fill these NaN values with the mean of the respective columns. This ensures that our data is clean and ready for analysis. We also split the data into features (X) and target variable (y), followed by dividing the dataset into training and testing sets. To standardize the feature variables, we use the StandardScaler.

In the EDA phase, we visualize the distribution of the target variable to understand the balance of the dataset. We also create a correlation matrix to identify relationships between different features. This helps in understanding which features might be more influential in predicting diabetes.

We then proceed to model building and training. We initialize three different models: Logistic Regression, Random Forest Classifier, and Support Vector Machine (SVM). Each model is trained on the training dataset and evaluated on the testing dataset. We use accuracy, precision, recall, and F1 score as our evaluation metrics. By comparing these metrics, we can determine which model performs the best for our task.

After training the models, we evaluate their performance. We create a confusion matrix for the best-performing model to understand the classification results in detail. Additionally, we plot the ROC-AUC curve to visualize the trade-off between the true positive rate and the false positive rate. This helps in assessing the model's ability to distinguish between the positive and negative classes.

In conclusion, the Random Forest Classifier provided the best performance among the three models, achieving a balance between accuracy and interpretability. This project demonstrates the effective use of machine learning for predicting diabetes, which can have a significant impact on health management and lifestyle choices.
