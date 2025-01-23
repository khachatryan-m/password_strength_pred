# password_strength_pred
Predicting password strength using Logistic Regression

# Description
The aim of this project is to predict password strength purely based on Machine Learning algorithms and simple NLP feature engineering techiques. No neural networks are used in the ML model.

# Dataset
The data is stored in a SQLite db and accessed programmatically from the notebook. The dataset is named password_data.sqlite and can be downloaded from this repository or from its original source, Kaggle again named in the same way. The dataset has 100K rows and 2 columns: password and its strength. The passwords are labeled as "weak", "medium" and "strong".

# Required software
No special software is required to run the notebook. Only Jupyter notebook is used in the project with built-in Python libraries for data manupiulation and modeling.

# Modelling and Outcome
For feature engineering, TF-IDF (Term Frequency - Inverse Document Frequency) - a statistical technique is used to vectorize the words by calculating the relative frequency of terms in a document. TF - IDF is not a bad choice in this context, as we are dealing with passwords only and there's no specific need to count for the semantic meaning of the words in the text. Hence, no need for more advanced and complex models like BART.

For modelling, Logistic Regression is implemented. The model has an average accuracy of 80% and a weighted precision of 78%.

