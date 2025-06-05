 Task 7: Support Vector Machines (SVM)  
Dataset: Breast Cancer Wisconsin Dataset  
Objective: Use SVMs with linear and RBF kernels for binary classification.

---

 Overview  
In this project, we implement and evaluate Support Vector Machines (SVM) to classify tumors as malignant or benign. Both linear and non-linear (RBF kernel) SVMs are trained and compared. Hyperparameters are tuned using grid search, and optional visualization is done using PCA.

---

 Dataset Details  
- Source: scikit-learn's built-in `load_breast_cancer()` dataset  
- Target Variable: `target` (0 = malignant, 1 = benign)  
- Features: 30 numerical attributes based on cell nuclei features

---

 Tools Used  
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn

---

 Steps Performed  
1. Loaded and normalized the dataset using `StandardScaler`  
2. Split data into training and test sets  
3. Trained linear SVM using `SVC(kernel='linear')`  
4. Trained RBF SVM using `SVC(kernel='rbf')`  
5. Tuned `C` and `gamma` using `GridSearchCV`  
6. Evaluated using accuracy and classification report  
7. (Optional) Visualized the data using PCA for decision boundary understanding

---

 Evaluation  
- Linear SVM: Achieved high accuracy and clear separation  
- RBF SVM: Performed well, especially with optimal `C` and `gamma`  
- Grid Search: Helped find best parameters for RBF kernel  
- PCA Visualization: Aided in understanding class separability in 2D

---

 Conclusion  
SVM is a powerful algorithm for binary classification. While linear SVM works well for linearly separable data, the RBF kernel extends its capability to handle non-linear boundaries. Proper scaling and parameter tuning are critical for SVM performance.

