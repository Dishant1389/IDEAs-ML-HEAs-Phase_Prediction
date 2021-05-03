# IDEAs-ML-HEAs-Phase_Prediction
Database and code for reproducing work submitted to "Computational Materials Science"

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
Input file to fix model parameters. All parametrs for model are modified here. Make modifications only after "[" symbol.

project_name - A directory with this name will be created. All results will be stored here.

database - Write database input filename here

y - Column name in database that will be used as target (Don't change this)

x - Name of features to be included in model (these can be changed freely, but don't add space between feature names)

layer_units - 

activation_functions - 

loss_function -

optimizer -

learning_rate -

iterations -

save_after_iterations - 

check_acc - 

check_after_iterations


