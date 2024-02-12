# credit-risk-classification
## Dataset
The dataset, `lending_data.csv`, includes multiple features related to loan applications. The target variable is `loan_status`, indicating the health of the loan.

## Methodology
The project follows these steps:
1. **Data Preparation**: Loading the data, creating feature (`X`) and target (`y`) datasets, and splitting these into training and testing sets.
2. **Model Training with Original Data**: A logistic regression model is trained on the original dataset.
3. **Evaluation**: The model's performance is assessed using accuracy, precision, recall, and F1 score.
4. **Resampling**: The training data is balanced using `RandomOverSampler` to address class imbalance.
5. **Model Training with Resampled Data**: A logistic regression model is trained on the resampled dataset.
6. **Evaluation and Comparison**: The performance of the model trained on resampled data is evaluated and compared to the model trained on the original data.

## Results
- The model trained on original data showed high accuracy for the majority class but lower performance metrics for the minority class.
- After resampling, the model displayed improved recall for the minority class, indicating enhanced capability in identifying high-risk loans, with a slight trade-off in precision.

## Conclusion
Resampling techniques, such as oversampling the minority class, can significantly improve the performance of logistic regression models in predicting minority classes in imbalanced datasets. This approach led to a more balanced model capable of detecting high-risk loans more effectively.

## Requirements
- Python 3.x
- pandas
- numpy
- scikit-learn
- imbalanced-learn