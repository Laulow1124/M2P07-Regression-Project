# M2P07 Regression Project
--------

**The objective of the M2P07 Regression Project is to explore multiple regression models, in order to find a model that predicts the rental price most accurately.**

**The material applied from Module 2 will be the following:**
1. Feature Engineering and Data Preprocessing
2. Linear Regression
3. Polynomial Regression
4. Regularization

**M2P07 Regression Project has the following conditions:**
1. Project must include EDA section.
2. Project must include visualization.
3. Data must be cleaned and prepared.
4. Use Feature Engineering, if applicable.
5. Must compare at minimum 3 regression models.
6. Explain which feature(s) are chosen for final model.
7. Use final model to make new predictions based on my provided input.

**The outline for the project will be the following:**

**The project will be split into five parts:**
1. Part 1 will involve EDA, Visualization, Data Cleaning, Encoding, Data Preparation (ex: Split to X and y).  <br>
2. Part 2 will be working with Model #1: Simple Linear Regression. <br>
3. Part 3 will be working with Model #2: Polynomial Regression. <br>
4. Part 4 will be working with Model #3: Polynomial Regression, with RidgeCV L2 Regularization. <br>
5. Part 5 will be determining which of the three models has the best performance and having the best performing model be our final model. <br>
   The final model will be used to make a prediction and includes some final comments/conclusion. <br>

**Conditions checklist:**
1. Project must include EDA section.
   - Found in Part 1 in M2P07 project notebook.
   - Checked number of null values, dtypes for each column, etc.
2. Project must include visualization.
   - Found in Part 1 and Part 5 in M2P07 project notebook.
   - Includes bar plots and scatterplots in Part 1.
   - Includes regression plot in Part 5.
3. Data must be cleaned and prepared.
   - Found in Part 1 in M2P07 project notebook.
   - Missing string values were replaced with the mode in the string columns.
   - Missing numerical values were replaced with the mean in the numerical columns.
   - Data preparation includes splitting data into X and y. (Later put into X_train, X_test, y_train and y_test). 
4. Use Feature Engineering, if applicable.
   - Used encoding (OneHotEncoder) for nominal categorical data. Found in Part 1 in M2P07 project notebook.
   - Used scaling (StandardScaler) for two models. Found in Part 2 (Model 1) and Part 4 (Model 3) in M2P07 project notebook. 
5. Must compare at minimum 3 regression models.
   - The three regression models to be compared: Simple Linear Regression, Polynomial Regression and Polynomial Regression with RidgeCV L2 Regularization.
   - Part 2 will be working with Model #1: Simple Linear Regression.
   - Part 3 will be working with Model #2: Polynomial Regression.
   - Part 4 will be working with Model #3: Polynomial Regression with RidgeCV L2 Regularization.
   - Part 5 will compare performance of all three models.
6. Explain which features are chosen for final model.
   - Found in Part 5 in M2P07 project notebook.
   - Final model was Simple Linear Regression.
   - Features for final model included encoding (OneHotEncoder) for nominal categorical data and scaling (StandardScaler).
7. Use final model to make new predictions based on my provided input.
   - Found in Part 5 in M2P07 project notebook.
   - As per prediction experimentation (In part 5.5 Final Model: Prediction in notebook), with input of "sq_feet" at 3000 and if the type is a 'House', the predicted price is $4296.2312. 

## Conclusion 
In conclusion, three models were tested: Simple Linear Regression, Polynomial Regression and Polynomial regression with Ridge L2 Regularization. <br>
**Of the three models, Simple Linear Regression had the best performance due to having the best metrics and was chosen to be the final model.** <br>
- Simple validation was used for all three models. The reason is so we could evaluate the metrics in a similar method before choosing final model.
- All three regression models required the data to be converted into numerical format hence the use of encoding. With the categorical data mainly being nominal, OneHotEncoder was used to convert categorical values to numerical values.
- With what was stated above, the final model (Simple Linear Regression) had the encoding feature (OneHotEncoder) applied to the data and hence why it was used as part of feature engineering.  
- Continuing with features, standard scaling was chosen in the final model as scaling as it was used due to the vast range of different numerical values for certain features (ex: sq_feet).
- As per prediction experimentation (In part 5.5 Final Model: Prediction), with input of "sq_feet" at 3000 and if the type is a 'House', the predicted price is $4296.2312. 
