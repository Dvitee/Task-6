# Task 6: KNN Classification on Iris Dataset

## Objective

The goal of this task is to apply the **K-Nearest Neighbors (KNN)** algorithm to classify flower species in the **Iris dataset** using only the first two features: sepal length and sepal width. A 2D decision boundary is visualized to understand the classification regions created by KNN.

---

## Dataset

The **Iris dataset** contains 150 samples from three species of Iris flowers:
- Iris Setosa
- Iris Versicolor
- Iris Virginica

Each sample includes 4 features:
- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

In this task, only the first two features are used for visualization purposes.

---

## Steps Performed

1. **Data Loading**: The Iris dataset is loaded from scikit-learn's built-in datasets.
2. **Feature Selection**: Only `sepal length` and `sepal width` are selected.
3. **Standardization**: The two selected features are standardized using z-score normalization.
4. **Model Training**: A KNN classifier with `k=5` is trained on the standardized data.
5. **Decision Boundary Plotting**: A mesh grid is generated to visualize decision regions in 2D, showing how KNN separates the data based on class labels.

---

## Output Visualization

A decision boundary plot is produced that shows how the KNN model (with k=5) separates the Iris species based on sepal length and width. Each region in the plot corresponds to a predicted class.

---

## Observations

- The model perfectly classifies the Iris Setosa class, which is linearly separable from the others.
- There is visible overlap between the Versicolor and Virginica classes, indicating that sepal features alone are not enough for perfect classification.
- The KNN algorithm is sensitive to the choice of `k` and the scale of features, which is why standardization is important.
- Using more features (e.g., petal measurements) would improve accuracy but reduce 2D interpretability.

---

## Conclusion

This task demonstrated how KNN works with low-dimensional data and how it creates decision boundaries based on class proximity. It also highlighted the importance of feature selection and preprocessing for meaningful visualization.

