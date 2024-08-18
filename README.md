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
- The model's performance is evaluated using metrics like accuracy, recall, precision, F1-score, and the ROC curve.
- A confusion matrix is visualized to observe the model's performance on the test data.

## Feature Importance
- Feature importance is computed to identify which features contribute most to predicting forest fires.

## Decision Tree Visualization
- The final decision tree is visualized to provide insights into the decision-making process of the model.

## Conclusion
This project successfully develops a predictive model to determine the likelihood of forest fires using environmental data from specific Algerian regions. The model could potentially be used by local authorities for better resource allocation and fire prevention strategies.
