# Digit Classification using SVM & KNN


##  Project Structure

- **Part A** – SVM and KNN model building and evaluation  
- **Part B** – FAISS vs Sklearn KNN (speed comparison)  
- **Part C** – Interview preparation (concepts + coding + debugging)  
- **Part D** – AI-assisted visualization and kernel trick explanation  

---

##  Dataset

The dataset used is **sklearn.datasets.load_digits**, which contains:

- 1797 grayscale images of handwritten digits (0–9)  
- Each image is 8×8 pixels (flattened into 64 features)  

---

##  Workflow

1. Load dataset  
2. Train-Test Split (80/20)  
3. Feature Scaling using StandardScaler  
4. Model Training:
   - SVM (RBF kernel with GridSearchCV)  
   - KNN (optimal K selection)  
5. Model Evaluation:
   - Accuracy  
   - Confusion Matrix  
   - Classification Report (Precision, Recall, F1-score)  

---

##  Models Used

### SVM (Support Vector Machine)
- Uses RBF kernel for non-linear decision boundary  
- Tuned using GridSearchCV (C and gamma)  
- Works well in high-dimensional space  

### KNN (K-Nearest Neighbors)
- Instance-based learning algorithm  
- Finds nearest neighbors using distance metric  
- Sensitive to feature scaling  

---

##  Results

- SVM achieved high accuracy (~98%)  
- KNN achieved slightly lower accuracy (~97%)  
- SVM performed better in capturing complex patterns  

---

##  Confusion Analysis

Commonly confused digit pairs:
- (3, 8)  
- (4, 9)  
- (1, 7)  

These errors occur due to visual similarity in handwritten digits.

---

##  FAISS vs KNN (Part B)

- FAISS is optimized for large-scale similarity search  
- Faster than sklearn KNN for large datasets  
- Accuracy remains comparable  

---

##  AI-Augmented Insights (Part D)

### Visualization:
- Demonstrates how SVM decision boundary changes with parameter **C**  
- Low C → simpler model (high bias)  
- High C → complex model (high variance)  

### Kernel Trick:
- Enables SVM to handle non-linear data  
- Uses similarity functions instead of explicit transformations  

---

##  Key Learnings

- Importance of feature scaling in SVM and KNN  
- Difference between margin maximization and distance-based learning  
- Hyperparameter tuning impact (C, gamma, K)  
- Confusion matrix analysis for model improvement  

---

##  Tools & Libraries

- Python  
- NumPy  
- Pandas  
- Scikit-learn  
- Matplotlib  
- FAISS  

---

##  How to Run

1. Open notebook in Google Colab  
2. Run all cells sequentially  
3. Analyze outputs and performance  

---

##  Author

**Hiten Mistry**
