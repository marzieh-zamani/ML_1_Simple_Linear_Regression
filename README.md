# Project 1: Simple Linear Regression
Simple linear regression on Fish.csv dataset.

## Code Breakdown
### Step 1: Define function_1 to estimate parameters for simple linear regression (‘intercept’ & ‘slope’)
`function_1` accepts a column of data ‘input_feature’ and another column ‘output’ and returns the Simple Linear Regression parameters ‘intercept’ and ‘slope’.
`intercept, slope = function_1(input_feature, output)`

### Step 2: Define function_2 to predict the model output using the simple linear regression parameters
`function_2` accepts a column of data ‘input_feature’, the ‘slope’, and the ‘intercept’ you learned, and returns a column of predictions ‘predicted_output’ for each entry in the input column.
`predicted_output = function_2(input_feature, intercept, slope)`

### Step 3: Define function_3 to calculate the RSS
`function_3` accepts a column of data: ‘input_feature’, and ‘output’ and the regression parameters ‘slope’ and ‘intercept’ and outputs the Residual Sum of Squares (RSS).
`RSS = function_3(input_feature, output, intercept, slope)`

### Step 4: Import fish data from Fish.csv
1. Importing fish data from Fish.csv using panda.read_csv function;
2. Converting Panda data to Numpy data;
3. Random spliting the data into 80% training and 20% test data (train_feature, test_feature, train_output, test_output);
4. Saving input features and output weigth separately;

### Step 5: Use function_1 to estimate model parameters (‘intercept’ & ‘slope’)
Use the above function to estimate the slope and intercept on the training data to predict weight of fish for each one of the following (one at a time) inputs. 
Then, save each model (slope and intercept) separately.‘Weight of the fish’ will be the ‘output’ and each of the following as an ‘input_feature’:
5.a. Length1 (Vertical Length in cm)
5.b. Length2 (Diagonal Length in cm)
5.c. Length3 (Cross Length in cm)
5.d. Height (cm)
5.e. Width (Diagonal width in cm)

### Step 6: Use function_2 to predict model output 
Using above estimated slopes and intercepts for each of model, fit a line through training data points. Draw separate plot for each of the ‘input_feature’.

### Step 7: Use function_3 to calculate model RSS
Calculate the RSS for all models.
Plot the RSS vs input_features for training and test data.

## Main files to check
The main file to check is the Jupyter notebook where:
- The functions are defined;
- The data is given;
- Then, the functions are called;
- The results are displayed and saved.

## Setup
Install [Miniconda](https://conda.io/miniconda).
Then, run the jupyter notebook in the "code" folder.

## Acknowledgment and References
This project has been developed based on the assignment provided by Dr. Abdul Bais, P.Eng. (abdul.bais@uregina.ca), my instructor for the course “ENEL-865/ENSE 865: Applied Machine Learning”.

This assignment is based on the first assignment of Machine Learning Regression course (from Coursera). 

- Dr. Abdul Bais, P.Eng. (abdul.bais@uregina.ca) page: 
https://www.uregina.ca/engineering/faculty-staff/faculty/bais-abdul.html

## Dataset
Download the Fish Market Dataset from Kaggle (https://www.kaggle.com/aungpyaeap/fish-market) to estimate weight of fish. Random split data into 80% training and 20% test data.

## My contribution
All scripts are written by my self.
______________
Marzieh Zamani