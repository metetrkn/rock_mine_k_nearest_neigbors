# KNN Project Exercise

    In this project, we are using the Sonar dataset to detect the difference between a rock or a mine based on the response of 60 separate sonar frequencies. The dataset contains the response metrics for 60 separate sonar frequencies sent out against a known mine field (and known rocks) and is labeled with the known object they were beaming the sound at (either a rock or a mine).

## Data Exploration

    A heatmap of the correlation between the difference frequency responses was created. The top 5 correlated frequencies with the target/label were identified.
    Train | Test Split

    The data was split into features and labels, and then into a training set and test set, with 90% for Cross-Validation training, and 10% for a final test set.
    Pipeline and GridSearch

    A pipeline was created that contains both a StandardScaler and a KNN model. A grid search was performed with the pipeline to test various values of k, and the best performing parameters were reported.
    Plotting Mean Test Scores

    A plot of the mean test scores per K value was created using the .cv_results_ dictionary.
    Final Model Evaluation

    Using the grid classifier object, a final performance classification report and confusion matrix were obtained. The model performed well in distinguishing between rocks and mines based on the sonar frequency responses.

## Confusion Matrix:

[[ 9  3]
 [ 0 10]]

## Classification Report:

                  precision    recall  f1-score   support

               M       1.00      0.75      0.86        12
               R       0.77      1.00      0.87        10

        accuracy                           0.86        22
       macro avg       0.88      0.88      0.86        22
    weighted avg       0.90      0.86      0.86        22

    This analysis demonstrates the effectiveness of KNN and the use of pipelines and GridSearchCV in creating a machine learning model capable of detecting the difference between a rock or a mine based on the response of the 60 separate sonar frequencies.

### Contributing

    Contributions are welcome. Please open an issue or submit a pull request to suggest changes or improvements.


### Credits

    Mete Turkan
    linkedIn : linkedin.com/in/mete-turkan
    Inst : m_trkn46
