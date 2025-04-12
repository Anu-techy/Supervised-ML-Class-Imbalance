**Class Imbalance** in ML occurs when the no of samples in each class is not equal leading to a skewed distribution.

Class Imbalance (one class majority, other class minority) is generally found in

1. Customer churn prediction
2. Cancer Prediction
3. Device Failure Prediction
4. Credit Card Fraud

**Ways to Handle Class Imbalance**

Under-sampling the Majority Class

                        Description: Reduces the number of samples in the majority class.

                        Pros: Faster training, balances dataset.

                        Cons: Potential loss of valuable data and patterns from the majority class.

Over-sampling the Minority Class (Simple Duplication)

                        Description: Replicates existing minority class samples to match the majority.

                        Pros: Easy to implement, preserves information.

                        Cons: Can lead to overfitting due to repeated samples.

SMOTE (Synthetic Minority Over-sampling Technique)

                        Description: Generates synthetic samples of the minority class using k-nearest neighbors.

                        Pros: Reduces overfitting risk by creating new, unique samples.

                        Cons: Can introduce noise, especially in high-dimensional or overlapping class spaces.

SMOTE + Tomek Links

                        Description: Combines SMOTE with Tomek links to clean up ambiguous boundary points.

                        If a majority and minority class instance are each other's nearest neighbors (a Tomek link), the majority class sample is removed.

                        Pros: Improves decision boundaries by removing borderline or overlapping examples.

                        Cons: Slightly more complex, requires additional computation.

Ensemble Methods

                        Description: Combines multiple models trained on balanced subsets of data (e.g., Balanced Bagging, EasyEnsemble).

                        Pros: Often achieves better generalization; robust to overfitting.

                        Cons: More computationally expensive, harder to interpret.

