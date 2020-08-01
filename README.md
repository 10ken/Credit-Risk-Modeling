# Credit-Risk-Modeling

The dataset was cleaned, encoded, explored, and visualized in credit-log-modelling.ipynb. 

------------------------------------------------------------------------------------------

train: 70%
test_set:30%

------------------------------------------------------------------------------------------

The logistic model had an initial accuracy of 81%. 
It was improved to an accuracy of 83% after finding an optiminal default probability.
The accuracy of the model was imporved to once more to 86% leveraging principal component analysis and hyperparamter turning.
There were 14 components from the encoded dataset, cr_clean2.

The data was also summarized with pivot tables.

------------------------------------------------------------------------------------------------

To furthur improve the predicted accuracy, a gradient boosted tree was developed with cr_clean2. 
The gradient boosted tree had an initial accuracy of 93.5% with all 27 features. 
The most important features were identified and the rest was removed.
The updated tree reduced the complexity by 12 features and had an accuracy of 93.3%.
