# neural-network-challenge-2
Module 19 Challenge
1. Accuracy as a Metric
Accuracy may not be the optimal metric for this data, particularly for predicting attrition:

Attrition Prediction: Attrition data is often imbalanced, where only a small percentage of employees leave. A model could achieve high accuracy by predicting most employees stay, without necessarily performing well on identifying actual leavers. Instead, metrics such as precision, recall, or F1 score would likely provide better insights into the model’s effectiveness.

Department Prediction: If department data is relatively balanced, accuracy could be appropriate. However, if certain departments are overrepresented, accuracy might still yield skewed results.

2. Activation Functions
For this branched neural network, the activation functions are chosen based on the target output types:

Attrition Prediction (Binary Classification): A sigmoid activation function is used. It outputs probabilities between 0 and 1, making it suitable for binary classification, helping the model make clear predictions about employee attrition.

Department Prediction (Multi-Class Classification): A softmax activation function is appropriate here, as it outputs a probability distribution across multiple classes, allowing the model to select the most probable department for an employee.

3. Potential Model Improvements
Consider the following adjustments to enhance model performance:

Hyperparameter Tuning: Refining the learning rate, batch size, and number of epochs could lead to better results.

Additional Layers or Units: Adding layers or units, both shared and branch-specific, could increase the model’s complexity and help capture nuanced patterns, especially if underfitting is detected.

Regularization: Techniques like dropout or L2 regularization can prevent overfitting and improve generalization.

Data Augmentation & Feature Engineering: Adding or engineering features, along with balancing the dataset, can help the model learn more effectively, especially for class imbalance issues.

Advanced Evaluation Metrics: Additional metrics, such as precision, recall, F1 score for binary classification, and possibly AUC-ROC for attrition prediction, would offer more granular insights and support further model tuning.
