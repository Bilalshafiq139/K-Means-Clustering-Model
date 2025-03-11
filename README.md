# K-Means-Clustering-Model
This repository contains a Python script that applies K-Means Clustering to a dataset about Facebook Live sellers in Thailand.


# K-Means Clustering Model

## Overview
This repository contains a Python script that applies **K-Means Clustering** to a dataset about **Facebook Live sellers in Thailand**. The model groups sellers into clusters based on engagement metrics such as reactions, comments, and shares.

---

## **Problem Statement**
Businesses using Facebook Live often want to segment their sellers based on audience engagement. This project uses **K-Means Clustering** to identify groups of sellers with similar interaction patterns, helping businesses tailor their marketing strategies accordingly.

### **Dataset Description**
The dataset used in this project is from [**UCI Machine Learning Repository: Facebook Live Sellers in Thailand**](https://archive.ics.uci.edu/dataset/488/facebook+live+sellers+in+thailand) and includes the following features:
- **Status Type**: Type of post (Photo, Video, etc.).
- **Number of Reactions**: Total reactions received.
- **Number of Comments**: Total comments received.
- **Number of Shares**: Total shares received.
- **Other Attributes**: Additional engagement metrics.

---

## **How the Script Works**
1. **Data Preprocessing**:
   - Loads the dataset and drops unnecessary columns (`status_id`, `status_published`).
   - Converts categorical `status_type` into numerical values using **Label Encoding**.
2. **Feature Scaling**:
   - Uses **MinMaxScaler** to scale numerical features between 0 and 1.
3. **K-Means Clustering**:
   - Applies **Elbow Method** to determine the optimal number of clusters.
   - Tests different cluster numbers (e.g., 2, 3, and 4) to compare results.
   - Assigns cluster labels to each seller.
4. **Visualization & Analysis**:
   - Plots **Elbow Method graph** to determine the best cluster count.
   - Uses **Scatter Plots** to visualize clusters based on engagement metrics.
   - Computes **Cluster Summary Statistics**.
5. **Export Results**:
   - Saves the clustered dataset as `Clustered_Live_20210128.csv` for further analysis.

---

## **Dependencies**
Ensure you have the following Python libraries installed:
```sh
pip install numpy pandas matplotlib seaborn scikit-learn
```

---

## **How to Run the Script**
1. Clone the repository:
   ```sh
   git clone <repository_url>
   ```
2. Navigate to the project folder:
   ```sh
   cd <project_folder>
   ```
3. Run the Python script:
   ```sh
   python k_means_clustering_.py
   ```
4. Follow the output to view clustering results and visualizations.

---

## **Contributing**
Contributions are welcome! Feel free to fork this repository and submit a pull request with improvements or additional features.


