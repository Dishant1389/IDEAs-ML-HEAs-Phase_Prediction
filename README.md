# IDEAs-ML-HEAs-Phase_Prediction
Accompanying dataset and code for article "Learning phase selection and assemblages in High-Entropy Alloys through a stochastic ensemble-averaging model" - Not published yet

Authors: Dishant Beniwal, Pratik K. Ray

## Contents

### File "db_HEAs.csv":
Database file - 323 HEAs with their phase information and normalized feature values.


### File "run_ANN_phase_prediction.py":
Creates ANN model using parameters defined in "Input_ANN.txt" file. A new directory is created to store trained models and training/validation results.

Requirements|recommended versions: 
Python|3.8.1 ; 
pandas|1.0.3 ; 
numpy|1.18.2 ; 
scikit-learn|0.22.2 ; 
tensorflow|2.2.0rc2 ; 
keras|2.3.1

### File "Input_ANN.txt":
Input file to define all the model parameters. Make modifications only after "[" symbol.

project_name - A directory with this name will be created. All results will be stored here.

database - Write database input filename here.

y - Column name in database that will be used as target (Don't change this).

x - Name of features to be included in model (these can be changed freely, but don't add space between feature names), feature added here must be present as a column in "db_HEAs.csv" file.

layer_units - No. of units in sequential hidden layers; This also controls no. of hidden layers; last layer is output layer (3 units, don't change this).

activation_functions - Activation function for sequential hidden layers; last layer is output layer (softmax, don't change this).

loss_function - Loss function used for error quantification (we used BinaryCrossentropy).

optimizer - Optimizer used for loss minimization (we used RMSprop).

learning_rate - Learning rate in backward propagation (we used contant lr=0.0005)

iterations - No. of iterations for which model will run (we used 5000).

save_after_iterations - No. of iterations after which current model will be saved (we used 100 i.e. model state is saved after every 100 iterations).

check_acc - Threshold accuracy that must be attained after (check_after_iterations); otherwise model will re-initialize all parameters and will start from beginnning. This ensures that model will either converge or will restart.

check_after_iterations - No. of iterations after which threshold accuracy will be checked.


