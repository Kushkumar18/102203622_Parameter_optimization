# 102203622_Parameter_optimization
## 🧠 Parameter Optimization with NuSVC on Dry Bean Dataset

### 📌 Objective
This project focuses on optimizing the hyperparameters of the Nu-Support Vector Classification (NuSVC) model using the Dry Bean Dataset. The goal is to evaluate different kernel and `nu` combinations to achieve the best classification accuracy through repeated random trials.

---

## 📂 Dataset Summary
- **Dataset**: Dry Bean Dataset  
- **Source**: UCI Machine Learning Repository  
- **Samples**: 13,611  
- **Features**: 16 numerical shape descriptors  
- **Target**: Type of dry bean (e.g., BARBUNYA, SIRA, SEKER)

---

## ⚙️ Workflow Steps

1. **Data Preprocessing**  
   - Encode categorical labels into numeric form using `LabelEncoder`
   - Scale the features using `StandardScaler` for consistent performance

2. **Hyperparameter Space**  
   - Kernels: `linear`, `rbf`, `poly`, `sigmoid`  
   - `nu`: Randomly selected from a defined range (0.01 to 0.3)

3. **Optimization Strategy**  
   - Random search across parameters  
   - Run each experiment multiple times with different `train_test_split` seeds  
   - Store and compare the best performing parameters from each run

4. **Evaluation**  
   - Accuracy Score on the test set  
   - Visualize convergence behavior of accuracy over iterations

---

## 🧪 Tools & Libraries
- `pandas`, `numpy` for data handling  
- `scikit-learn` for modeling, preprocessing, and evaluation  
- `matplotlib` for plotting convergence graphs  
- `tqdm` for progress monitoring (optional)

---

