# Forest-Fire-Prediction-using-Decision-Trees
The GitHub project utilizes decision trees to predict forest fires using the Algerian Forest Fires Dataset obtained from the UCI Machine Learning Repository.

## Dataset Overview
The project utilizes the Algerian Forest Fires dataset from the UCI Machine Learning Repository. This dataset includes 244 instances encompassing data from two regions of Algeria, namely the Bejaia region in the northeast and the Sidi Bel-abbes region in the northwest, covering the period from June to September 2012.

[Dataset link](https://archive.ics.uci.edu/dataset/547/algerian+forest+fires+dataset)

## Libraries Required
- Pandas
- NumPy
- Seaborn
- Matplotlib
- scikit-learn

## Data Preprocessing
- Data is loaded and cleaned of null values.
- The 'Classes' feature is encoded into binary labels: 'fire' as 1 and 'not fire' as 0.
- Irrelevant features such as 'year', 'DMC', 'DC', 'FWI', and 'BUI' are dropped based on correlation analysis.

## Exploratory Data Analysis
- Correlation heatmap is generated to understand the relationships between features.

## Model Building
- A DecisionTreeClassifier is employed.
- GridSearchCV is used to tune hyperparameters and find the best model settings based on accuracy.
- The model is trained using the optimized parameters.

## Model Evaluation
- The model's performance is assessed using various metrics: accuracy, recall, precision, F1-score, and confusion matrix.
- The AUC ROC curve is plotted to evaluate the model's ability to distinguish between classes, providing a comprehensive view of performance across different thresholds.
- **Performance Metrics:**
  - **Accuracy:** 0.9672131147540983
  - **Confusion Matrix:**
    ```
    [[26  2]
     [ 0 33]]
    ```
  - **Recall:** 1.0
  - **Precision:** 0.9428571428571428
  - **F1 Score:** 0.9705882352941176
- These results show how well the model can predict forest fires, highlighting its robustness in correctly identifying fire instances.

## Feature Importance
- Feature importance is computed to identify which features contribute most to predicting forest fires.

## Decision Tree Visualization
- The final decision tree is visualized to provide insights into the decision-making process of the model.

## Conclusion
This project successfully develops a predictive model to determine the likelihood of forest fires using environmental data from specific Algerian regions. The inclusion of the AUC ROC curve and detailed performance metrics provides a thorough assessment of the model's effectiveness, making it a valuable tool for local authorities in fire prevention and resource allocation strategies.
