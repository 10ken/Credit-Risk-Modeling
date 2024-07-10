# Credit-Risk-Modeling:

Based on the dataset, despite the current application measures taken, 18.4% of clients defaulted for the first time and 37.81% of clients who had previously defaulted, defaulted again.

The credit risk modeling project aimed to predict loan defaults with high accuracy and reliability by prioritizing the improvement of recall without significantly compromising precision and accuracy, thereby minimizing risk for both lenders and applicants.

The project involved multiple stages:
  **1.** Data Cleaning
  
  **2.** Exploration
  
  **3.** Development Of Various Models To Enhance Predictive Performance.

## Final Results

The multi-agent model improved the recall, actual defaulters, by 31% while having insignificant impacts to the precision and accuracy.

![Model Performance](https://github.com/10ken/Credit-Risk-Modeling/blob/master/img/all_performance_KPIs.png)

## Summary of Findings
**Model Name:**     |     **Recall**  |  **Precision**  |  **Accuracy**   
                    
**Log Model:**      |    53       |   73      |    93   

**XGB Model:**     |     72    |      94     |     93

**Multi-Agent Model:**     |     84     |     70    |      90

- **Data Cleaning and Exploration**: Essential for understanding the dataset and preparing it for modeling.
-Certainly! Here are the improved versions of each statement:
- **Logistic Regression and PCA**: Improved model accuracy from 81% to 86%, but recall was only 53% despite an optimized threshold.
- **Gradient Boosted Trees**: Achieved 93.3% accuracy with reduced model complexity, and improved recall and precision by 20%.
- **Multi-Agent Model**: Boosted recall by 31%, focusing on reducing false negatives and accurately identifying potential defaulters without significantly compromising precision or accuracy.

### Performance Metric Definitions
- **Recall**: Measures the proportion of actual defaulters, minimizing false negatives

- **Precision**: Measures the proportion of predicted defaulters, minimizing false positives.
  
- **Accuracy**: Measures the proportion of correctly identified instances, minimizing both false positives and false negatives.


Below is a comprehensive summary highlighting the process, performance metrics, improvements, and notable points.

## Data Preparation and Exploration

The dataset was cleaned, encoded, explored, and visualized in the initial stages. The data cleaning process involved handling missing values, outlier removal, and one-hot encoding of categorical variables. The data exploration included generating pivot tables and visualizations to understand the current credit risk situation better.

## Model Development and Performance

### Logistic Regression Model

- **Initial Performance**: The logistic model achieved an initial accuracy of 81%.
- **Improvements**:
  - **Probability Threshold Optimization**: By optimizing the default probability threshold, accuracy improved to 83%.
  - **Principal Component Analysis (PCA)**: Leveraging PCA and hyperparameter tuning, the accuracy was further enhanced to 86%. Fourteen components from the encoded dataset (cr_clean2) were used in this step.
  
### Gradient Boosted Trees Model

- **Initial Performance**: A gradient boosted tree model was developed using cr_clean2, achieving an initial accuracy of 93.5% with all 27 features.
- **Feature Importance**: The most important features were identified, reducing the model complexity by removing 12 less significant features.
- **Updated Performance**: The updated tree achieved an accuracy of 93.3%.

### Multi-Agent Model

A new addition to the project involved the development of a Multi-Agent model, which combined the predictions of logistic regression and gradient boosted trees to further enhance predictive performance.

- **Focus on Recall**: This model prioritized reducing false negatives—accurately identifying clients who would default on their loans—while placing less emphasis on reducing false positives.
- **Performance Metrics**:
  - **Accuracy and Precision**: The overall accuracy and precision decreased by 3%.
  - **Recall Improvement**: Recall increased significantly by 31%, improving the detection of actual defaulters.
  - **Threshold Optimization**: An optimal threshold of 0.45 improved recall by 5%, from 48% to 53%, without impacting accuracy.
  - **Final Recall**: Further optimization led to a recall improvement to 55% without compromising accuracy.

### Model Insights

- **Top Features**: The top five most important features for determining a loan default were the applicant's income, age, employment length, and the loan's interest rate and amount.
- **Default Rate Reduction**: With the Multi-Agent model, the default rate would decrease from 22% to 7%, resulting in minimized risk for both the lender and the applicant.
