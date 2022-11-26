# Income qualification
## Problem Statement Scenario:
Many social programs have a hard time ensuring that the right people are given enough aid. It’s tricky when a program focuses on the poorest segment of the population. This segment of the population can’t provide the necessary income and expense records to prove that they qualify.
In Latin America, a popular method called Proxy Means Test (PMT) uses an algorithm to verify income qualification. With PMT, agencies use a model that considers a family’s observable household attributes like the material of their walls and ceiling or the assets found in their homes to
classify them and predict their level of need.
While this is an improvement, accuracy remains a problem as the region’s population grows and poverty declines.
The Inter-American Development Bank (IDB)believes that new methods beyond traditional econometrics, based on a dataset of Costa Rican household characteristics, might help improve PMT’s performance.
## Task:
To create a model that considers a family’s observable household attributes like the material of their walls and ceiling or the assets found in their homes to classify them and predict their level of need.
## Dataset:
The dataset consists of 33413 records and 143 features.
## Approach:
  - Identified the output variable.
  - Rectified biases in the dataset using SMOTE.
  - Checked whether all members of the house have the same poverty level.
  - Checked if there is a house without a family head.
  - Set poverty level of the members and the head of the house within a family.
  - Identified null values existing in columns and treated them appropriately.
  - Removed null value rows of the target variable.
  - Performed Dimensionality reduction using recursive feature elimination and reduced the number of features to 5.
  - Predicted the accuracy using random forest classifier.
  - Checked the accuracy using random forest with cross validation and found it as 90.4
