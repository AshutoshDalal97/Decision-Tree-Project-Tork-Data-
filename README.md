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
Class	          Meaning
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

# Model Insights
Decision Tree with Gini (73.4%) performs slightly better than Entropy (70.7%)
