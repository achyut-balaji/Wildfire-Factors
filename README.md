# Wildfire-Factors


My project is about using a specific parameter to predict different parameters which affect wildfires.
My parameters are :
X and Y: Map coordinates (1 to 9)
Month and Day: Calendar month and day of the week
FFMC, DMC, DC, ISI: FWI codes and indices tracking moisture and spread rate
Temp, RH, wind, rain: Temperature, humidity, wind, and rain metrics
area: Total burned area in hectares (target variable)

My project used two  tree-based modeling techniques: a Decision Tree and a Random Forest. The single Decision Tree model was utilized first to establish a transparent, easily interpretable baseline for data behavior. Random Forests usually deliver better performance by reducing overfitting and capturing more complex patterns. Comparing the simple logic of a single tree against the aggregated power of the forest allowed for a thorough evaluation of accuracy versus model explainability.

My final result was that of the Random Forest Model performing better than Decision Tree.

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

The following image was the MAE of my random forest:
<img width="616" height="292" alt="image" src="https://github.com/user-attachments/assets/8a4193c3-b0d0-4e09-8659-b303acd8f243" />
The following image is the r^2 for random forest:
<img width="1583" height="522" alt="image" src="https://github.com/user-attachments/assets/96a140cd-e36b-4730-a827-4fd59b4a53a3" />
The next image is for the decision tree model:

<img width="641" height="164" alt="image" src="https://github.com/user-attachments/assets/9f24127b-6f9b-4ca7-8ee7-6860e382e4f8" />

This next series of pictures is for the decision tree model:

<img width="138" height="834" alt="image" src="https://github.com/user-attachments/assets/47ccc489-aee0-4004-afb7-7a720d4a0ff4" />

These are my predictions for random forest:

<img width="150" height="858" alt="image" src="https://github.com/user-attachments/assets/b79830a0-8082-4fd3-b527-942fc29825b6" />


<img width="150" height="858" alt="image" src="https://github.com/user-attachments/assets/e4257c76-4c2d-4ca4-99e4-ff45cd135888" />

<img width="97" height="403" alt="image" src="https://github.com/user-attachments/assets/a89ee88d-d801-4ea2-95c9-e01a445bea1d" />

 My data was sourced from Kaggle and came from a national park in Portugal.
