## Project Summary: Machine Efficiency Classification

### Objective:
The goal of this project is to build a predictive model that classifies the **Efficiency Status** of industrial machines (`Low`, `Medium`, `High`) using a rich set of sensor and operational features. This falls under a **multiclass classification** problem.

---

### Dataset Overview:
- The dataset contains **machine-level metrics**, including:
  - `Temperature_C`, `Vibration_Hz`, `Power_Consumption_kW`
  - `Network_Latency_ms`, `Packet_Loss_%`, `Error_Rate_%`, etc.
  - Target variable: `Efficiency_Status` (categorical)
- Total samples: _(100000)_
- Features include both **numeric and categorical** values, preprocessed appropriately.

---

### Exploratory Data Analysis (EDA):
- Distribution plots, pairplots, and heatmaps were used to understand feature relationships.
- Correlation matrix highlighted strong relationships between:
  - `Power_Consumption_kW` and `Production_Speed_units_per_hr`
  - `Error_Rate_%` and `Quality_Control_Defect_Rate_%`
- Scatter plots revealed patterns in how efficiency levels relate to key metrics.

---

### Models Applied:
- Linear Regression (optional implemented just to check the accuracy)
- Logistic Regression
- Naive Bayes
- Support Vector Machine (SVC)
- Decision Tree Classifier
- Random Forest Classifier
- K-Nearest Neighbors (KNN)

 All models were evaluated using **accuracy** and confusion matrices.

A separate section explored **SVC decision boundaries**, visualizing class separation in 2D space using selected features.

---

###  Clustering (Unsupervised Learning):
Although the task is supervised, **K-Means clustering** was performed to:
- Discover hidden groupings within the data
- Compare cluster assignments to true `Efficiency_Status` labels
- Visualize clusters using PCA (or 2D feature plots)

This provided **additional insight** into the natural structure of the data.

---

###  (Optional) Regression Extension:
An additional experiment involved treating `Efficiency_Status` as a **numeric target** (`Low`=0, `Medium`=1, `High`=2), applying regression models to predict efficiency levels as a continuous outcome. This showcases flexibility in framing the problem.

---

### Visualizations Included:
- Heatmaps & pairplots
- Scatter plots with hue, size, and custom palettes
- Decision boundary plot (SVC)
- Clustering plot (KMeans)
- Distribution plots

---

### Conclusion:
- The classification models achieved solid performance, with **Random Forest and SVC** giving the highest accuracy.
- Visual insights and clustering validated the predictive structure of the data.
- The project effectively demonstrates a full data science workflow — from preprocessing and EDA, to modeling, evaluation, and interpretability — using both supervised and unsupervised techniques.

---
