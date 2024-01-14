# Data Preprocessing and Binary Classification


### Data Source
We will focus on predicting the survival of Titanic passengers. We have access to training data in the file `data.csv` and evaluation data in the file `evaluation.csv`.

## Feature List
- `survived`: Whether the passenger survived (0 = No, 1 = Yes) - target variable to predict
- `pclass`: Class of the ticket (1 = first, 2 = second, 3 = third)
- `name`: Name
- `sex`: Gender
- `age`: Age in years
- `sibsp`: Number of siblings/spouses on board
- `parch`: Number of parents/children on board
- `ticket`: Ticket number
- `fare`: Ticket price
- `cabin`: Cabin number
- `embarked`: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)
- `home.dest`: Residence/Destination

## Given Task

1. Load the data from the `data.csv` file into a notebook. Divide it into subsets for training, validation, and testing.
2. Conduct basic data preprocessing:
   - Transform features for use in the chosen classification model.
   - Optionally create new features based on existing ones.
   - Handle missing values appropriately, avoiding methodological errors.
   - Utilize visualizations with concise and proper commentary.
3. Apply a decision tree and k-nearest neighbors to the prepared data. For each model:
   - Comment on the suitability of the model for the given task.
   - Select key hyperparameters for tuning and find their optimal values.
   - Calculate the F1 score, plot the ROC curve, and determine the AUC. Be cautious about methodological errors.
   - Provide thorough commentary on the obtained results.
4. Choose the final model from the tested options in the previous step. Estimate the expected accuracy on new data not previously available. Beware of methodological errors.
5. Load the evaluation data from the `evaluation.csv` file. Use the final model to make predictions for these data (the target variable is no longer present). Create a `results.csv` file with two columns: ID, survived. Submit this file alongside the notebook.

Example of the first rows in the `results.csv` file:
```
ID,survived
1000,0
1001,1
...
```