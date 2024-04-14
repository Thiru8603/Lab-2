Project Title: Student Passing Outcome Prediction Extraction

Description:

This R script performs logistic regression analysis to predict whether a student will pass based on their studied credits and IMD band (a measure of academic performance). The script includes data preprocessing steps, handling of unseen credit levels (optional), model building and evaluation, and the option to create a visualization.

Prerequisites:

R software: https://www.r-project.org/foundation/
ggplot2 package (optional, for visualization): Install within R using install.packages("ggplot2")
Instructions:

Data Loading and Preprocessing:

Ensure the CSV file containing student data (studentS.csv) is located in the same directory as this script.
Edit the script to replace "C:\\Users\\thiru\\Downloads\\studentInfo.csv" with the actual path to your CSV file.
The script performs data cleaning and feature engineering steps, including converting categorical variables and creating a numeric scale for the IMD band.
Handling New Credit Levels (Optional):

The script can identify rows in the test data that have unseen credit values not present in the training data.
You can choose to:
Correct these values manually if you have knowledge of the appropriate credit levels.
Remove these rows from the test data if necessary.
Combining Credit Levels (Optional):

The script allows you to combine existing credit levels into broader categories if it makes sense for your analysis.
Edit the script to define new credit level ranges and update both training and test data accordingly.
Re-training Model with All Data (Optional):

By default, the script splits the data into training and test sets (80%/20%).
You can choose to combine all data for training if you don't need a separate test set.
Building and Evaluating the Model:

The script builds a logistic regression model using the glm function in R.
It calculates model coefficients, significance levels, and overall accuracy based on predicted vs. actual outcomes in the test data.
Visualization (Optional):

The script includes commented-out code for creating a bar chart comparing predicted and actual outcomes using the ggplot2 package.
Uncomment this section and customize the visualization as needed.
Additional Notes:

Consider feature engineering (creating new features) to potentially improve model performance.
Explore other model evaluation metrics beyond accuracy, such as precision, recall, F1-score, or ROC AUC.
Fine-tune the model by adjusting hyperparameters (e.g., regularization) or data preprocessing techniques.
Contributing:

Feel free to submit pull requests with improvements or extensions to this script.
