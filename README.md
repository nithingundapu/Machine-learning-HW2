# Machine-learning-HW2
#700772575
#Nithin Gundapu
Q7. Decision Tree on Iris 
 I trained Decision Tree models with depths 1, 2, and 3. 
- Depth=1: Accuracy was low on both training and test sets → clear underfitting. 
- Depth=2–3: Accuracy improved greatly (96–99% train, 91–93% test). Good fit without much loss of generalization. 
- Deeper trees: Would likely overfit (train=100%, test drops). Conclusion: A depth of 2–3 is best, giving strong performance without overfitting

Q8. kNN with Two Features
 Using only sepal length and width, I trained kNN models with k=1, 3, 5, and 10 and plotted the decision boundaries. 
- k=1: Very jagged boundaries, the model memorizes training points → overfitting. 
- k=3: Boundaries smoother, capturing class structure better.
 - k=5: Even more stable, best trade-off between bias and variance. 
- k=10: Boundaries overly smooth, class details lost → underfitting. 
Conclusion: Small k → high variance (overfit), large k → high bias (underfit). Best results around k=3–5.

Q9. Performance Evaluation of kNN (k=5) 
- Confusion Matrix: Few misclassifications, mostly between Versicolor and Virginica. 
- Accuracy: ≈93%. - Precision, Recall, F1: All above 0.90 → balanced performance.
 - ROC Curves & AUC: AUC ≈0.95–0.98 for all classes → strong separability. 
Conclusion: kNN with k=5 performs very well, with high accuracy and excellent ROC/AUC value

Overall Summary 
- Decision Tree: Depth 1 underfits, depth 2–3 is optimal, very deep trees risk overfitting. 
- kNN: k=1 overfits, k=10 underfits, best around k=3–5. 
- Performance: kNN (k=5) achieves ≈93% accuracy with strong evaluation metrics, making it a reliable classifier for Iris
