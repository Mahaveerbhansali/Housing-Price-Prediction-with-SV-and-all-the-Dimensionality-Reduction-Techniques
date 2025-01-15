Housing Price Prediction with SVM and Dimensionality Reduction Techniques
This project uses various dimensionality reduction techniques to improve the accuracy of housing price prediction through Support Vector Machines (SVM).

1. Overview
This project focuses on predicting housing prices based on various features, such as location and median income, using Support Vector Machines (SVM). The project explores several dimensionality reduction techniques, such as PCA, LDA, ICA, and FDA, to improve model performance and reduce computational complexity.

2. Data
The dataset is sourced from housing data, which includes information such as:

Longitude & Latitude

Housing median age

Total rooms

Total bedrooms

Population

Households

Median income

Ocean proximity

The target variable is the median house value.

3. Model: Support Vector Machine (SVM)
SVM is a powerful supervised learning algorithm used for regression and classification tasks. For this project, the SVM is employed to predict housing prices based on the input features.

Kernel Selection
SVM models use different types of kernels, such as:

Linear Kernel
Polynomial Kernel
Radial Basis Function (RBF) Kernel
Model Evaluation
Mean Squared Error (MSE) is used to evaluate the model's performance.
Learning Curve is plotted to assess the training vs. validation error across various training sizes.
SVM Evaluation Function:
The function evaluate_svm_kernels() evaluates the model with different kernels and compares their Mean Squared Error (MSE) on the test data.

4. Dimensionality Reduction Techniques
To improve computational efficiency and potentially enhance performance, several dimensionality reduction techniques are applied:

PCA (Principal Component Analysis)
Reduces the dimensionality of the dataset while retaining as much variance as possible.
Graph: The explained variance ratio for each component is plotted, showcasing the amount of information each principal component retains.
LDA (Linear Discriminant Analysis)
Focuses on maximizing the separability between classes by reducing the dimensionality.
Graph: The LDA projection of the data is visualized to see how the model separates the target variable.
ICA (Independent Component Analysis)
A method to separate mixed signals into statistically independent components.
Graph: ICA components are plotted, providing insight into the features' independence.
LLE (Locally Linear Embedding)
A non-linear dimensionality reduction technique that preserves the local neighborhood structure.
Graph: Scatter plot of LLE projections, showing how well it maintains local relationships in the data.
FDA (Fisher Discriminant Analysis)
A supervised technique to reduce dimensions by maximizing class separability.
Graph: FDA projection, showing how the categories of the target variable are predicted.
MDA (Maximum Margin Discriminant Analysis)
A variation of LDA focusing on maximizing the margin between classes.
5. Visualizations
SVM Kernel Comparison
A bar plot compares the MSE results for each kernel used in the SVM model.
Learning Curves
Plots the training and validation error as the number of training samples increases, providing insight into model performance.
Decision Boundaries
Decision boundaries are visualized using the first two principal components after reducing the dimensionality via PCA. This allows for a better understanding of how the SVM is classifying data in lower dimensions.
Dimensionality Reduction Comparison
A bar plot compares the performance (MSE) of various dimensionality reduction techniques, highlighting which technique provides the best results.
6. Results
The project evaluates the impact of each dimensionality reduction technique on the performance of the SVM model.
Summary: Dimensionality reduction techniques like PCA, ICA, and FDA are evaluated, and their effectiveness is compared based on the MSE.
7. Installation & Usage
To use this repository:

Install required libraries:

bash
Copy code
pip install -r requirements.txt
Run the Jupyter Notebook:

bash
Copy code
jupyter notebook SVM_DR.ipynb

8. Conclusion
This project demonstrates the effectiveness of combining SVM with dimensionality reduction techniques for housing price prediction. The results indicate that different dimensionality reduction methods impact model performance, and techniques like PCA and LDA show notable improvements.
