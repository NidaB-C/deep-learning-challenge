# Alphabet Soup Charity Success Prediction

## Overview of the Analysis

The purpose of this analysis is to use machine learning and neural networks to help Alphabet Soup—a philanthropic foundation—predict the success of grant applications. By analyzing a dataset of more than 34,000 organizations that have previously received funding, we aim to build a binary classifier model that can predict whether applicants will be successful if funded by Alphabet Soup.

## Results

### Data Preprocessing

- **Target Variable(s):** The target for our model is the `IS_SUCCESSFUL` column, which indicates whether the money was used effectively.
- **Feature Variables:** Features include `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, and `ASK_AMT`.
- **Non-Feature Variables:** The `EIN` and `NAME` columns were removed from the input data as they do not contribute to the outcome of `IS_SUCCESSFUL`.

### Compiling, Training, and Evaluating the Model

- **Model Configuration:** The neural network model includes an input layer, multiple hidden layers with 80, 50, and 30 neurons respectively, and an output layer. The activation functions used are ReLU for the hidden layers and Sigmoid for the output layer.
- **Achieving Target Model Performance:** The original model did not meet the target performance of 75% accuracy. After optimization, adjustments including additional hidden layers, adjusting neurons, and experimenting with different activation functions were made.
- **Optimization Attempts:** To enhance model performance, we adjusted the number of neurons and layers, experimented with different activation functions, and modified the input data preprocessing steps. These attempts included more detailed binning of categorical variables and the removal of less impactful features.

### Summary

The final model showed an improvement in accuracy, indicating a better prediction capability for the success of charity applications funded by Alphabet Soup. However, it still did not consistently exceed the 75% accuracy target. 

**Recommendation for a Different Model:** For further improvement, a Random Forest Classifier could be explored. This model could potentially solve the classification problem more effectively due to its ability to handle non-linear data and provide a higher accuracy by averaging multiple decision trees that individually consider random subsets of features.

## Conclusion

This project demonstrates the power and flexibility of deep learning for predictive analytics in philanthropic funding. Despite challenges in achieving the desired accuracy, the analysis provides a foundation for future exploration and model optimization. The use of alternative models like Random Forest Classifier offers a promising direction for enhancing prediction accuracy and ultimately aiding Alphabet Soup in making more informed funding decisions.
