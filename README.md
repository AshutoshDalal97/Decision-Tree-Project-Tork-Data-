# Decision-Tree-Project-Tork-Data
📌 Project Overview

This project focuses on predicting the balance state of a scale using machine learning techniques. The dataset is based on the physical principle of torque, where the balance depends on weights and their distances from the pivot.

The goal is to classify whether the scale tilts:

Left (L)
Right (R)
Balanced (B)

# Dataset Information

This dataset is sourced from the UCI Machine Learning Repository.

# Features:
left-weight	             (Weight on the left side);
left-distance	           (Distance from pivot (left));
right-weight	           (Weight on the right side) and
right-distance	        ( Distance from pivot (right))

# Target Variable:

   L	             (Left side is heavier)
   R	            (Right side is heavier)
   B	             (Balanced)

# Underlying Concept

The dataset follows the physics rule:
Torque = Weight \times Distance

If Left Torque > Right Torque → L
If Right Torque > Left Torque → R
If equal → B

# Machine Learning Task
Type: Supervised Learning
Problem: Multi-class Classification
Algorithms Used:
Decision Tree Classifier

# Model Evaluation
Accuracy Score
Confusion Matrix
Classification Report

# Model Comparison
Decision Tree --> 74.4 % (Gini criterion)
Extra Trees --> 84.8%
Random Forest --> 87.2% 
Gradient Boosting --> 89.6%
XGBoost --> 89.6%
SVM --> 95.2%

🔍 Performance Summary
Decision Tree showed the lowest performance due to class imbalance
Ensemble methods (Random Forest, Extra Trees) significantly improved accuracy
Boosting models (Gradient Boosting, XGBoost) further enhanced performance (~89.6%)
SVM achieved the highest accuracy (~95.2%)

🧠 Key Insights
SVM with a linear kernel performed best, indicating that the dataset is nearly linearly separable
Tree-based models struggled initially with the minority class (B), but performance improved with ensemble techniques
SVM successfully classified all classes, including the minority class, with high precision and recall


🏆 Final Conclusion

SVM with a linear kernel is the most suitable model for this dataset, achieving the highest accuracy and balanced performance across all classes. The results suggest that the dataset has a well-defined and nearly linear decision boundary.
