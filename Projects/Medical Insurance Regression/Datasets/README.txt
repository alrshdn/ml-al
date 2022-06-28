Model type: Regression model
Independent variables: age, sex, bmi, children, smoker, region
Dependent variable: charges

Data types before proccessing:
age (int)
sex (string) {male, female}
bmi (float)
children (int)
smoker (string) {yes, no}
region (string) {northeast, northwest, southeast, southwest}
charges (float)

Data types after proccessing:
age (int)
sex (one-hot encoding) {male, female}
bmi (float)
children (int)
smoker (one-hot encoding) {yes, no}
region (one-hot encoding) {northeast, northwest, southeast, southwest}
charges (float)

Data Normalization: MinMaxScalar

Activation function: None

Data source:
https://github.com/stedy/Machine-Learning-with-R-datasets/blob/master/insurance.csv