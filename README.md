# **Image Clustering using K-Means**

## **Overview**
This project implements **K-Means clustering** for **unsupervised image clustering**, using **Principal Component Analysis (PCA)** and **U-MAP** for dimensionality reduction. The dataset consists of **10,740 images**, where each image is represented by **740 numerical pixel values** (0-255). The best clustering performance achieved a **V-score of 0.62**.

---

## **Approach**
### **1. Data Preprocessing**
- **Dimensionality Reduction**:
  - **PCA (2 components)** for feature reduction.
  - **U-MAP** for better cluster separation.
- **Data Normalization**:
  - Standard Scaler was used for normalization.

### **2. K-Means Clustering**
- **Random initialization of centroids**.
- **Manhattan distance** was chosen as the best metric (V-score = 0.62).
- Clusters were assigned based on distance minimization.

### **3. Evaluation Metrics**
- **Silhouette Score** was used to determine the best `k` value.
- **Best k-values**:
  - `k=4` → **0.4995**
  - `k=12` → **0.4719**
  - `k=16` → **0.4736**

### **4. Final Parameter Selection**
| Distance Metric | V-Score |
|----------------|--------|
| Manhattan      | 0.62   |
| Euclidean      | 0.61   |
| Cosine Similarity | 0.53   |

📌 **Manhattan distance was selected** due to the highest clustering performance.

---

## **Implementation Details**
### **K-Means Pseudocode**
1. **Initialize `K` centroids randomly**.
2. **Assign points to the nearest centroid**.
3. **Recalculate centroids** by computing the mean of each cluster.
4. **Repeat until convergence** (centroids stop changing or max iterations reached).
5. **Return final clusters**.

---

## **Execution Steps**
1. 📥 **Upload dataset (10,740 images as numerical values).**
2. 🔍 **Run PCA (2 components) & U-MAP for dimensionality reduction.**
3. 🏷️ **Apply K-Means clustering & evaluate performance.**
4. 📊 **Visualize clusters and analyze metrics.**

---

## **Results & Insights**
- **Best clustering performance achieved V-score = 0.62**.
- **Manhattan distance performed better than Euclidean & Cosine Similarity.**
- **PCA + U-MAP improved cluster separation** and visualization.

---

## **Future Work**
- 🔬 **Experiment with other clustering techniques** (e.g., DBSCAN, Spectral Clustering).
- 🚀 **Try deep learning-based clustering methods** (e.g., Autoencoders).
- 📈 **Tune hyperparameters further** to optimize cluster separation.

---

## **Author**
👤 **Preethi Ranganathan**  
📧 [prangana@gmu.edu](mailto:prangana@gmu.edu)  

---

