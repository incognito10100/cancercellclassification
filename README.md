

# Cancer Cell Classification using Scikit-Learn

## Project Overview

This project focuses on building a machine learning model to classify cancer cells as malignant or benign. Using the Breast Cancer Wisconsin (Diagnostic) dataset from Scikit-Learn, the model predicts the type of cancer cell based on features extracted from cell nuclei in biopsy images.

## Dataset Description

The dataset consists of 30 features computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. These features describe characteristics of the cell nuclei present in the image. The target variable is binary, representing whether the cancer is malignant (1) or benign (0).

**Key Features:**
- Radius (mean, worst)
- Texture (mean, worst)
- Perimeter (mean, worst)
- Area (mean, worst)
- Smoothness (mean, worst)
- Compactness (mean, worst)
- Concavity (mean, worst)
- Concave points (mean, worst)
- Symmetry (mean, worst)
- Fractal dimension (mean, worst)

## Project Workflow

1. **Data Preprocessing**
   - **Data Loading**: The dataset is loaded using Scikit-Learn’s `load_breast_cancer()` function.
   - **Data Splitting**: The data is split into training (80%) and testing (20%) sets.
   - **Feature Scaling**: Features are standardized to improve model performance.

2. **Model Training**
   - **Algorithm**: A Support Vector Machine (SVM) classifier is chosen for this task.
   - **Training**: The SVM model is trained using the training set.

3. **Model Evaluation**
   - **Testing**: The trained model is evaluated on the test set.
   - **Metrics**: The following metrics are calculated:
     - **Accuracy**
     - **Precision**
     - **Recall**
     - **F1 Score**
   - **Classification Report**: A detailed report of precision, recall, and F1 score for each class is generated.

## Model Performance Summary

Here’s a summary of the model's performance on the test data:

- **Accuracy**: 97.37%
- **Precision**: 97.22%
- **Recall**: 98.59%
- **F1 Score**: 97.90%

### Classification Report:

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0 (Benign) | 0.98      | 0.95   | 0.96     | 43      |
| 1 (Malignant) | 0.97      | 0.99   | 0.98     | 71      |

- **Overall Accuracy**: 97% on the test set.
- **Macro Average**: Precision: 0.97, Recall: 0.97, F1-Score: 0.97
- **Weighted Average**: Precision: 0.97, Recall: 0.97, F1-Score: 0.97

## Conclusion

The SVM model performs well on the Breast Cancer Wisconsin dataset, with an accuracy of 97% and high precision and recall scores. This indicates that the model is highly effective at distinguishing between malignant and benign cancer cells.


## References

- [Breast Cancer Wisconsin (Diagnostic) Dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html)
- [Scikit-Learn Documentation](https://scikit-learn.org/stable/documentation.html)

