# Identify Customer Segments

This project applies **unsupervised learning techniques** to identify customer segments for a mail-order sales company in Germany. The goal is to determine which segments of the general population are most similar to the company’s existing customer base, enabling **targeted marketing campaigns** that maximize returns.

The data is provided by **Bertelsmann Arvato Analytics** and represents a real-world customer segmentation challenge.

---

## Project Overview

- **Objective:** Use clustering techniques on demographic data to discover segments of the population that align with the company’s core customers.  
- **Dataset:**  
  - `Udacity_AZDIAS_Subset.csv` – General population demographics (≈ 890k rows × 85 features).  
  - `Udacity_CUSTOMERS_Subset.csv` – Company customers demographics (≈ 191k rows × 85 features).  
  - `Data_Dictionary.md` – Feature descriptions.  
  - `AZDIAS_Feature_Summary.csv` – Summary of feature properties.  

---

## Workflow

1. **Data Loading & Exploration**  
   - Load population and customer datasets.  
   - Explore feature summary and data dictionary.  

2. **Data Preprocessing**  
   - Handle missing values (replace special codes with `NaN`).  
   - Drop columns with excessive missing data.  
   - Encode categorical variables appropriately.  
   - Normalize / standardize numerical features.  

3. **Dimensionality Reduction**  
   - Apply **PCA** to reduce dataset dimensionality while retaining variance.  

4. **Clustering**  
   - Apply **K-Means clustering** on the transformed data.  
   - Determine optimal cluster number (e.g., using the elbow method).  

5. **Customer Segmentation**  
   - Assign both general population and customer data to clusters.  
   - Compare distributions to identify **over-represented clusters** among customers.  

6. **Insights & Applications**  
   - Document clusters that represent the **core customer base**.  
   - Provide recommendations for targeted marketing strategies.  

---

## Technologies Used

- **Python 3**  
- **Libraries:**  
  - `pandas`, `numpy` – Data manipulation  
  - `matplotlib`, `seaborn` – Visualization  
  - `scikit-learn` – PCA, clustering, preprocessing  

---

## Usage

1. Clone this repository or download the notebook.  
2. Place the provided dataset files in the project folder.  
3. Open the notebook:

   ```bash
   jupyter notebook Identify_Customer_Segments.ipynb
   ```

4. Run cells step by step to reproduce the analysis.  

---

## Results

- Segments of the German population were identified based on demographic attributes.  
- Comparison of clusters showed which groups are **over-represented among existing customers**.  
- Insights can be used to **improve marketing campaign targeting**.  

---

## Author

This project is part of the **Udacity Machine Learning Nanodegree**.  
