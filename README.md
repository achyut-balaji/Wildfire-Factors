# Wildfire-Factors


My project is about using a specific parameter to predict different parameters which affect wildfires.
My parameters are :
X and Y: Map coordinates (1 to 9)
Month and Day: Calendar month and day of the week
FFMC, DMC, DC, ISI: FWI codes and indices tracking moisture and spread rate
Temp, RH, wind, rain: Temperature, humidity, wind, and rain metrics
area: Total burned area in hectares (target variable)

My project used two  tree-based modeling techniques: a Decision Tree and a Random Forest. The single Decision Tree model was utilized first to establish a transparent, easily interpretable baseline for data behavior. Random Forests usually deliver better performance by reducing overfitting and capturing more complex patterns. Comparing the simple logic of a single tree against the aggregated power of the forest allowed for a thorough evaluation of accuracy versus model explainability.

My final result was that of the Random Forest Model performing.

I also used multiple libraries:

| Library                   | Module / Class          | Purpose                                                                                                      |
| ------------------------- | ----------------------- | ------------------------------------------------------------------------------------------------------------ |
| pandas                    | pd                      | Data manipulation and analysis using DataFrames.                                                             |
| numpy                     | np                      | Numerical computing and array operations.                                                                    |
| collections               | Counter                 | Counts the frequency of items in a list or dataset.                                                          |
| matplotlib.pyplot         | plt                     | Creates graphs, charts, and visualizations.                                                                  |
| graphviz                  | graphviz                | Draws decision trees and other graph structures.                                                             |
| IPython.display           | display, HTML           | Displays formatted tables, HTML, and other outputs in Jupyter notebooks.                                     |
| sklearn.model_selection   | train_test_split        | Splits data into training and testing sets.                                                                  |
| sklearn.ensemble          | RandomForestRegressor   | Machine learning model for regression using a random forest.                                                 |
| sklearn.metrics           | accuracy_score          | Measures classification accuracy.                                                                            |
| sklearn.metrics           | classification_report   | Provides precision, recall, F1-score, and support for classification models.                                 |
| sklearn.metrics           | confusion_matrix        | Shows the performance of a classification model in matrix form.                                              |
| sklearn.metrics           | mean_squared_error      | Measures regression error by calculating the average squared difference between predicted and actual values. |
| sklearn.metrics           | r2_score                | Calculates the coefficient of determination (R²) for regression models.                                      |
| sklearn.tree              | export_graphviz         | Exports decision trees to Graphviz format for visualization.                                                 |
| sklearn                   | tree                    | Contains decision tree algorithms and visualization tools.                                                   |
