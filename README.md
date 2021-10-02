# Neural_Network_Charity_Analysis
## Overview
The purpose of this analysis was to create a neural network that evaluates whether an applicant for funding through Alphabet Soup should be successful.

## Resources
- Data Source: [Historic Projects](https://github.com/mcarson16/Neural_Network_Charity_Analysis/blob/main/Resources/charity_data.csv)
- Software: Jupyter Notebooks

## Results
### Data Pre-Processing
- Target Variable: "IS_SUCCESSFUL"
- Features:
  - APPLICATION_TYPE: 17 categorical values 
  - AFFILIATION: 6 possible affiliations 
  - CLASSIFICATION: 70 categories
  - USE_CASE: 5 cases 
  - ORGANIZATION: 4 types of organizations
  - STATUS: 1 or 0 for active or inactive
  - INCOME_AMT: Ranges of income of the organizations that were funded.
  - SPECIAL_CONSIDERATIONS: yes or no
  - ASK_AMT: How much money was requested and granted.
- Columns Dropped: EIN and NAME

### Compiling, Training, and Evaluating the Model
- The initial model contained two hidden layers. The first was created with 80 neurons, the second with 30. The ReLU activation function was used for both. For the output activation, a sigmoid function was chosen in accordance with the binary Target Variable.
- The initial model's accuracy level was approximately 73%.
- Attempted methods of optimization included adding an additional hidden layer, increasing the number of epochs for the model training, and changing the activation to LeakyReLU. However, none of these attempts were able to reach the goal threshhold of 75% accuracy. There was no appreciable increase in model accuracy.

### Summary
- The model can accurately predict the majority of outcomes, but it did not reach the goal threshhold of 75% accuracy, even with adjustments. There may be factors that contribute to the success of applications that are not captured in the dataset. Alternatively, one may try using a logistic regression rather than a neural network to see if a simpler model could produce better results.
 
