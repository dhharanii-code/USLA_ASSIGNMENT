# USLA_ASSIGNMENT
# 🚗 Used Car Market Segmentation Using Unsupervised Learning

## 📌 Project Overview
This project uses Unsupervised Machine Learning to identify different segments in the used car market based on vehicle characteristics such as kilometres driven, fuel type, seller type, transmission, ownership and car age.

The project analyzes **3,577 used-car records** using three clustering algorithms:
- K-Means Clustering
- Hierarchical Clustering
- DBSCAN

Selling price and price category are excluded during model training and used only for interpreting the clusters.

## 🎯 Objectives
- Perform Exploratory Data Analysis (EDA).
- Preprocess numerical and categorical data.
- Identify the optimal number of clusters.
- Implement and compare clustering algorithms.
- Analyze and interpret the generated car segments.
- Visualize clusters using PCA.

## 📂 Dataset Description
- Dataset: `car.xlsx`
- Sheet: `Raw_data`
- Total Records: 3,577
- Total Columns: 10
- Missing Values: 0
- Duplicate Records: 0

### Features Used
| Numerical Features | Categorical Features |
|---|---|
| km_driven | fuel |
| car age | seller_type |
| | transmission |
| | owner |

## 🛠️ Technologies Used
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib

## ⚙️ Methodology
1. Data Loading and Exploration
2. Exploratory Data Analysis
3. Data Preprocessing
4. Feature Encoding and Scaling
5. Optimal Cluster Selection using Elbow Method and Silhouette Score
6. K-Means Clustering
7. Hierarchical Clustering
8. DBSCAN Clustering
9. Model Evaluation and Comparison
10. Cluster Profiling and PCA Visualization

## 📊 Model Performance

| Algorithm | Clusters | Silhouette Score | Davies-Bouldin Index | Calinski-Harabasz Score |
|---|---:|---:|---:|---:|
| K-Means | 10 | 0.2820 | 1.3069 | 804.2531 |
| Hierarchical | 10 | 0.2272 | 1.4969 | 581.7779 |
| DBSCAN | 13 | 0.3050 | 1.0009 | 447.5427 |

### Key Findings
- K-Means achieved the highest Calinski-Harabasz score and assigned all records to clusters.
- DBSCAN achieved the highest Silhouette Score and lowest Davies-Bouldin Index.
- DBSCAN identified 612 records (17.11%) as noise.
- K-Means identified 10 interpretable used-car segments.
- PCA's first two components explained 64.41% of the total variance.

## 🚀 How to Run the Project

**1. Clone the repository**
```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

**2. Navigate to the project folder**
```bash
cd used-car-market-segmentation
```

**3. Install dependencies**
```bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib openpyxl jupyter
```

**4. Open Jupyter Notebook**
```bash
jupyter notebook
```

**5. Run the notebook**

Open `Used_Car_Market_Segmentation_Analysis.ipynb` and execute all cells.

Make sure `car.xlsx` is in the same folder as the notebook.

## 📁 Project Structure
```text
Used-Car-Market-Segmentation/
│
├── Used_Car_Market_Segmentation_Analysis.ipynb
├── car.xlsx
├── Used_Car_Market_Segmentation_Project_Report.pdf
└── README.md
```

## 📈 Expected Outputs
- Exploratory Data Analysis visualizations
- Elbow Method graph
- Silhouette Score analysis
- DBSCAN tuning results
- Cluster assignments
- Cluster profiles
- PCA visualization
- Model evaluation comparison

## 🔮 Future Enhancements
- Test additional clustering algorithms.
- Improve cluster separation.
- Test different feature combinations.
- Validate the model using larger datasets.

## 📝 Conclusion
This project successfully identifies meaningful segments in the used-car market using unsupervised learning. K-Means provides complete segmentation, while DBSCAN helps identify dense groups and unusual records.

The results can help understand patterns in vehicle usage, ownership, age and market characteristics.

---

**Project Domain:** Machine Learning – Unsupervised Learning  
**Project Type:** Used Car Market Segmentation
