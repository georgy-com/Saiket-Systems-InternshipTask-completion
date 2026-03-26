The data preparation stage ensured that the dataset was clean, structured, and suitable for machine learning models.

The dataset initially contained 7043 entries and 21 features, with a mixture of categorical and numerical variables. A critical issue identified was that the TotalCharges column was stored as an object (string) rather than a numeric type. This could lead to errors in model training and statistical analysis. Converting it to a numeric ensured accurate computations.

Although initial checks showed no missing values, conversion of TotalCharges introduced 11 null values, which highlights an important insight:

- Data type inconsistencies can silently introduce missing values.

- Categorical variables were transformed using one-hot encoding, allowing machine learning models to interpret non-numeric data effectively.

Finally, splitting the dataset into training and testing sets ensured that:

- The model learns from one portion of data
- And is evaluated on unseen data This prevents overfitting and improves generalization.
- Key Insight:
Proper data preparation directly impacts model accuracy, reliability, and interpretability. Errors at this stage can propagate throughout the entire analysis.
