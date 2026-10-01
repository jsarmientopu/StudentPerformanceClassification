# Student Performance Classification

Machine learning project developed for a **Kaggle competition**, focused on predicting students' global academic performance from demographic, socioeconomic, and academic information.

The project explores different classification approaches, including **Random Forest, Neural Networks, and XGBoost**, with data preprocessing, model tuning, evaluation, and generation of the final Kaggle submission.

## Dataset

The project uses the **Kaggle competition dataset**, provided through `train.csv`. The training dataset contains **692,500 records** and includes information such as:

* Academic program and department
* Tuition and enrollment information
* Working hours
* Household socioeconomic conditions
* Internet and computer access
* Parents' education
* Other student and family characteristics

The target variable, `RENDIMIENTO_GLOBAL`, contains four performance categories:

* Low
* Medium-Low
* Medium-High
* High

The notebook performs data cleaning, missing-value treatment, categorical variable processing, and feature preparation before training the models.

## Models

The project compares several classification approaches:

### Random Forest

Used as a tree-based model and baseline for comparison, with different hyperparameter configurations evaluated.

### Neural Network

A fully connected neural network implemented with **TensorFlow/Keras**, with different architectures and training configurations explored.

### XGBoost

Used as the main approach, with hyperparameter tuning for parameters such as learning rate, tree depth, and `min_child_weight`.

## Kaggle Submission

After model selection and tuning, the final model is trained and used to predict the performance category for the **Kaggle test dataset**.

The notebook generates a **CSV submission file** containing the corresponding student IDs and predicted `RENDIMIENTO_GLOBAL` values, which can be uploaded directly to the competition.
