# dip-svm
DiP-SVM : Distribution Preserving Kernel Support Vector Machine for Big Data

In literature, the task of learning a support vector machine for large datasets has been performed by splitting the dataset into manageable sized “partitions” and training a sequential support vector machine on each of these partitions separately to obtain local support vectors. However, this process invariably leads to the loss in classification accuracy as global support vectors may not have been chosen as local support vectors in their respective partitions. We hypothesize that retaining the original distribution of the dataset in each of the partitions can help solve this issue. Hence, we present DiP-SVM, a distribution preserving kernel support vector machine where the first and second order statistics of the entire dataset are retained in each of the partitions. This helps in obtaining local decision boundaries which are in agreement with the global decision boundary, thereby reducing the chance of missing important global support vectors. We show that DiP-SVM achieves a minimal loss in classification accuracy among other distributed support vector machine techniques on several benchmark datasets. We further demonstrate that our approach reduces communication overhead between partitions leading to faster execution on large datasets and making it suitable for implementation in cloud environments.
