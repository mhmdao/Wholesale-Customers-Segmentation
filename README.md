# Wholesale Customers Segmentation

## 📌 Project Overview
This project applies clustering techniques to segment wholesale customers based on their purchasing behavior. The goal is to help the company understand different client segments, allowing them to better cater to and support each type.

## 📂 Dataset
We use the [Wholesale Customers Dataset](https://www.kaggle.com/datasets/binovi/wholesale-customers-data-set), which contains information about annual spending across different product categories for various customers, as well as channel & region for each client.

## 🎯 Objectives
- Scale the data for effective clustering.
- Apply three different clustering techniques:
  - K-Means Clustering
  - Hierarchical Clustering
  - DBSCAN (Density-Based Spatial Clustering of Applications with Noise)
- Compare the segments using silhouette score & domain intuition to determine the best segmentation.
- Predict the cluster of a new client based on their purchase behavior.

## 🛠️ Implementation Steps
### 1️⃣ Data Preprocessing
- Scale the features for better clustering performance.
- Explore data distributions and outliers.

### 2️⃣ Clustering Techniques
- Implement K-Means, Hierarchical, and DBSCAN clustering.
- Tune hyperparameters (e.g., number of clusters in K-Means).
- Visualize clusters. 

### 3️⃣ Evaluation & Selection
- Compute Silhouette Scores for each method.
- Use domain intuition to interpret segments.
- Select the best-performing clustering technique.

### 4️⃣ Prediction
- Predict the cluster of a new customer.

## 📊 Results & Insights
- K-Means with 3 clusters is chosen as our best model, based on sihouette_score(~0.46) as well as the decently sized clusters(cluster0: 350, cluster01: 53, cluster02: 37)
- Details of each group description could be found on section 6 of the project ipynb file.

## 🛠️ Technologies Used
- Python 🐍
- Pandas, NumPy 📊
- Scikit-learn 🤖 (for clustering and evaluation metrics)
- Matplotlib, Seaborn 📈 (for visualization)

## 🚀 How to Use
1. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/wholesale-customers-segmentation.git
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the clustering analysis:
   ```sh
   python clustering_analysis.py
   ```
4. Predict the cluster for a new client:
   ```sh
   python predict_cluster.py --input 'new_client_data.csv'
   ```

## 🔮 Future Work
- Implement additional clustering methods like Gaussian Mixture Models (GMM).
- Build a dashboard to visualize customer segments dynamically.
- Deploy the model using a web interface.

## 🤝 Contributing
Feel free to fork this repository, make improvements, and submit a pull request!

## 📝 License
This project is open-source and available under the [MIT License](LICENSE).
