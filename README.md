# Healthcare-stroke-prediction-RUDRA
AI project using Logistic Regression to predict stroke risk
# Healthcare Stroke Prediction Using Machine Learning

# 1. Project Overview

This project uses Artificial Intelligence and Machine Learning to predict whether a patient is likely to have a stroke based on healthcare information.

The project uses the Healthcare Stroke Prediction dataset and develops a Logistic Regression classification model using Python.

# 2. Project Objectives

- Explore and prepare a healthcare dataset.
- Identify patterns and relationships between patient information and stroke outcomes.
- Develop a Logistic Regression model to predict stroke cases.
- Evaluate the model using accuracy, precision, recall and F1-score.
- Improve the model by addressing class imbalance.

# 3. Technologies and Libraries Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn

# 4. Dataset

The project uses the Healthcare Stroke Prediction dataset, containing 5,110 patient records and information such as age, hypertension, heart disease, average glucose level, BMI and smoking status.

The target variable is `stroke`, where:
- 0 represents no stroke.
- 1 represents stroke.

# 5. Data Preparation

The dataset was prepared through the following steps:

- Removed unnecessary ID information.
- Checked for duplicate records and missing values.
- Replaced missing BMI values using median imputation.
- Encoded categorical variables using One-Hot Encoding.
- Standardised numerical features using StandardScaler.
- Divided the dataset into training and testing sets.
- Applied Random OverSampling to balance the training data.

# 6. Machine Learning Model

Logistic Regression was selected as the classification algorithm.

An initial model was trained using the original training distribution. A refined model was then trained using the balanced training dataset.

# 7. Model Results

| Metric | Initial Model | Refined Model |
|---|---:|---:|
| Accuracy | 95.21% | 74.46% |
| Precision | 100% | 13.75% |
| Recall | 2% | 80% |
| F1-score | 3.92% | 23.46% |

The refined model improved recall from 2% to 80%, allowing it to identify more actual stroke cases. However, it also produced more false positive predictions.

# 8. Limitations

The model has limitations, including low precision and false positive predictions. It has not been clinically validated and should not be used to make real medical decisions.

# 9. Future Improvements

Future improvements could include testing other machine learning algorithms, applying hyperparameter tuning, comparing different class-balancing techniques and evaluating the model using additional healthcare datasets.

# 10. How to Run the Project

1. Download the `.ipynb` notebook from this repository.
2. Open [Google Colab](https://colab.research.google.com/).
3. Upload the notebook.
4. Run the code cells in order.

# 11. Project Disclaimer

This project was developed for educational purposes. Its predictions are not intended for medical diagnosis or treatment.
