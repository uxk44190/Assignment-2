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

We trained a k-Nearest Neighbors model with k = 5 and checked how well it predicts flower species on a held-out test set. We report accuracy (overall correctness), a confusion matrix (where the model mixes up classes), and precision, recall, and F1 for each species (plus macro/micro averages). We also plot ROC curves in a one-vs-rest setup and compute AUC to show how well each class is separated.

How to read it: the confusion matrix tells you which species get confused most; high precision means few false alarms, high recall means few misses, and F1 balances both. Macro-averages treat all species equally; micro-averages weight by sample count. AUC closer to 1.0 means the class is easy to distinguish.

Deliverables: printed metrics, the confusion matrix, and per-class ROC curves with AUC.
Bottom line: use the matrix to spot confusions, F1 for balanced performance, and AUC to judge class separability.


