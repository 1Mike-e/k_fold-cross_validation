# k-Fold Cross Validation with Kernel SVM

This project demonstrates the implementation of **k-Fold Cross Validation** using a Kernel SVM classifier on the **Social Network Ads** dataset. The objective is to evaluate the model's performance more robustly and mitigate the impact of data split variability.

## 📂 Dataset

- **File:** `Social_Network_Ads.csv`
- **Features:**
  - `Age`
  - `Estimated Salary`
- **Target:**
  - `Purchased` (Binary: 0 or 1)

## 🧠 Model Overview

- **Classifier:** Support Vector Machine (SVM)
- **Kernel:** Radial Basis Function (RBF)
- **Validation:** 10-Fold Cross Validation

## 🚀 Project Workflow

1. **Library Imports**  
   Import required libraries such as `numpy`, `pandas`, `matplotlib`, and `scikit-learn`.

2. **Data Loading**  
   Load the dataset and split it into feature matrix `X` and target vector `y`.

3. **Train-Test Split**  
   Divide the data into training and testing sets (75% train, 25% test).

4. **Feature Scaling**  
   Normalize feature values using `StandardScaler`.

5. **Model Training**  
   Train an SVM classifier with an RBF kernel on the training set.

6. **Model Evaluation**  
   - Predict on the test set.
   - Compute and print the confusion matrix.
   - Calculate test accuracy.

7. **k-Fold Cross Validation**  
   Apply 10-fold cross validation to evaluate model stability.
   - Print mean accuracy and standard deviation.

8. **Visualization**  
   - Plot decision boundaries for both training and test sets using contour plots.
   - Display class separation visually.

## 📈 Results

- **Confusion Matrix**: Printed on the console
- **Test Accuracy**: Printed using `accuracy_score`
- **Cross-Validation Score**:
  - Mean Accuracy
  - Standard Deviation (variation across folds)

## 📊 Visual Output

Visualizations of decision boundaries are generated for:
- **Training Set**
- **Test Set**

These plots show how the SVM model separates the two classes based on Age and Estimated Salary.

## ⚙️ Dependencies

- Python 3.x
- NumPy
- pandas
- matplotlib
- scikit-learn

### Install with pip:

```bash
pip install numpy pandas matplotlib scikit-learn
