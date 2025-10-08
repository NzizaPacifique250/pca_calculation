# Principal Component Analysis (PCA) on Student Performance Factors

This notebook demonstrates the application of **Principal Component Analysis (PCA)** to a dataset of student performance factors.
PCA is a **dimensionality reduction technique** that transforms a set of correlated variables into a set of uncorrelated variables called *principal components*.

---

## Steps Covered

### 1. Load and Standardize the Data

* Load the dataset and standardize the numerical features.
* Standardization ensures that all features have a mean of 0 and a standard deviation of 1.

### 2. Calculate the Covariance Matrix

* Compute the covariance matrix of the standardized data to understand the relationships between features.

### 3. Perform Eigendecomposition

* Calculate the eigenvalues and eigenvectors of the covariance matrix.

  * **Eigenvalues** represent the variance explained by each principal component.
  * **Eigenvectors** represent the directions of the principal components.

### 4. Sort Principal Components

* Sort the eigenvectors based on their corresponding eigenvalues in descending order.
* Eigenvectors with higher eigenvalues capture more variance.

### 5. Project Data onto Principal Components

* Project the standardized data onto the selected principal components to reduce dimensionality.

### 6. Output the Reduced Data

* Display the shape and content of the reduced dataset.

### 7. Visualize Before and After PCA

* Visualize the data before and after PCA to observe the effect of dimensionality reduction.

---

## 📊 Dataset

The dataset used in this notebook is **`StudentPerformanceFactors.csv`**,
which contains various factors that may influence student performance.

---

## ⚙️ How to Run the Notebook

### 1. Clone the repository containing this notebook:

```bash
git clone https://github.com/NzizaPacifique250/pca_calculation.git
cd pca_calculcation
```

### 2. Install the required libraries:

```bash
pip install pandas numpy matplotlib
```

### 3. Open the notebook in a Jupyter environment such as:

* [Google Colab](https://colab.research.google.com/)
* Jupyter Notebook
* JupyterLab

### 4. Run the cells sequentially to perform the PCA analysis.

---

## 📈 Explained Variance and PCA

In PCA, the **explained variance** of each principal component is determined by its eigenvalue.
The **explained variance ratio** represents the proportion of the total dataset variance captured by each component.

By analyzing the **cumulative explained variance**, we can identify how many principal components are needed to retain a desired percentage of the original variance (e.g., **95%**).

This helps reduce dimensionality while preserving most of the important information in the data.
