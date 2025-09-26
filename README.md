# Assignment-1-

Question 7:

This script trains Decision Tree classifiers on the Iris dataset with
different depths (1, 2, 3) to compare training vs. testing accuracy.
It demonstrates the bias–variance trade-off:
- Very shallow trees (e.g., depth=1) may underfit and perform poorly.
- Deeper trees (e.g., depth=3) fit more patterns and improve train accuracy,
  but overly deep trees can overfit and hurt generalization.

Outputs:
- Train and test accuracy for each specified max_depth.

  

Question 8:

Objective
Build a k-Nearest Neighbors classifier using two Iris features (typically sepal length and sepal width) and visualize decision boundaries for multiple k values (e.g., k = 1, 3, 5, 10).

Data & Features
Use the Iris dataset with exactly two features for plotting in 2D. Common choice: sepal_length (x-axis) and sepal_width (y-axis). Encode targets as three classes: setosa, versicolor, virginica.

Procedure

Load Iris and select the two features (X ∈ ℝ²) and labels (y).

(Optional) Standardize features—useful if scales differ; with sepal features it’s less critical but still recommended for consistency.

For each k in {1, 3, 5, 10}:

Fit kNN on the selected two features.

Create a mesh grid over the feature range and predict class on each grid point.

Plot the decision region (background) and overlay the true data points with class colors and a legend.

Add axis labels and a concise title indicating the k value.




Question 9:

Split the data into train and test (e.g., 70/30) using stratification on the labels.

Train kNN with k=5 on the training set.

Predict class labels on the test set and obtain predicted probabilities for ROC/AUC.

Compute the confusion matrix (sklearn.metrics.confusion_matrix) and display it with class names (setosa, versicolor, virginica).

Report accuracy and print precision, recall, and F1 per class, including macro and micro averages (classification_report).

For multi-class ROC, binarize the labels (one-vs-rest), plot a ROC curve for each class using predicted probabilities, and compute per-class AUC; also report micro- and macro-average AUC.

Summarize key observations: which classes are most often confused, whether metrics are balanced across classes, and how separable the classes look from ROC/AUC.


