# IDEAs-ML-HEAs-Phase_Prediction
Database and code for reproducing work submitted to "Computational Materials Science"

Authors: Dishant Beniwal, Pratik K. Ray

## Contents

### File "db_HEAs.csv":
Database file - 323 HEAs with their phase information and normalized feature values.


### File "Input_ANN.txt":
Input file to fix model parameters. All parametrs for model are modified here. Make modifications only after "[" symbol.
project_name - A directory with this name will be created. All results will be stored here.
database - Write database input filename here
y - Column name in database that will be used as target (Don't change this)
x - Name of features to be included in model (these can be changed freely, but don't add space between feature names)
layer_units - 
