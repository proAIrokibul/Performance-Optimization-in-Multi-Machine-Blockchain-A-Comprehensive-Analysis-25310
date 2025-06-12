# Performance-Optimization-in-Multi-Machine-Blockchain-A-Comprehensive-Analysis-25310
## 📌 Project Overview

This project focuses on **analyzing and optimizing performance** in **multi-machine blockchain systems** using empirical benchmarking and classification modeling. We study how parameters like transaction send rates, block size, latency, and CPU usage interact to affect throughput and system reliability.

By leveraging **machine learning classification techniques**, we build predictive models that can detect and classify system states (e.g., stable vs. overloaded) — paving the way for smarter, self-tuning blockchain infrastructures.

---

## 🎯 Objectives

- Analyze blockchain node performance under stress-test scenarios.
- Benchmark latency, throughput, and CPU usage under different configurations.
- Build classifiers to predict system performance states based on observed metrics.
- Provide data-driven visual and predictive insights for system engineers.

---

## 📁 Dataset Overview

| Feature Name       | Description                                |
|--------------------|--------------------------------------------|
| `Set Send Rates`   | Configured transaction rate (TPS)          |
| `Send Rates`       | Actual transaction send rate               |
| `Block Size`       | Size of each block transmitted             |
| `Min Latency`      | Minimum observed latency                   |
| `Avg Latency`      | Average transaction confirmation latency   |
| `Max Latency`      | Peak observed latency                      |
| `Throughput`       | Processed transactions per second          |
| `CPU Usage (%)`    | CPU utilization per node                   |

- Total Records: `3081`
- Target Label: System performance state (classified from throughput using quantile bins)

---

## 🧪 Methodology

### 🧼 Data Preprocessing
- Handled scaling, normalization, and engineered a classification label using throughput bins.
- Split dataset into train and test sets for fair model evaluation.

### 📊 Exploratory Data Analysis
- Correlation heatmaps
- Scatter and pair plots of latency, throughput, and CPU usage
- 3D plots (CPU vs Latency vs Throughput)
- Histograms and box plots to detect anomalies

### 🤖 Classification Models Applied
1. **Random Forest Classifier**
2. **Support Vector Machine (SVM)**
3. **Gradient Boosting Classifier**

---

## 🧠 Model Results

### 🔍 Random Forest Classifier
- **Accuracy**: `96.76%`

| Class | Precision | Recall | F1-Score |
|-------|-----------|--------|----------|
|   0   |   0.94    |  0.97  |   0.95   |
|   1   |   1.00    |  1.00  |   1.00   |
|   2   |   0.96    |  0.94  |   0.95   |

---

### 🔍 Support Vector Machine
- **Accuracy**: `93.35%`

| Class | Precision | Recall | F1-Score |
|-------|-----------|--------|----------|
|   0   |   0.86    |  1.00  |   0.93   |
|   1   |   0.99    |  0.98  |   0.98   |
|   2   |   0.97    |  0.82  |   0.89   |

---

### 🔍 Gradient Boosting Classifier
- **Accuracy**: `95.62%`

| Class | Precision | Recall | F1-Score |
|-------|-----------|--------|----------|
|   0   |   0.93    |  0.96  |   0.95   |
|   1   |   0.99    |  0.99  |   0.99   |
|   2   |   0.95    |  0.92  |   0.93   |

---


## 💼 Business Impact

- 🏗 **Infrastructure Optimization**  
  Enables system engineers to preemptively identify stress conditions and optimize resource allocation.

- 🧠 **Predictive Monitoring**  
  Classifiers can be deployed in real-time environments to automatically flag performance degradation and recommend corrective actions.

- 💰 **Cost Efficiency**  
  Helps reduce unnecessary over-provisioning of compute resources and improves energy efficiency across blockchain nodes.

- ⚙️ **Smarter DevOps Pipelines**  
  Integrates with CI/CD systems to enable performance-aware deployment configurations.

