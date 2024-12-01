# Customer Segmentation with KMeans Clustering
## Project Overview
This project applies **KMeans clustering** to segment customers based on their behavior and interaction with products or services. The dataset is pre-processed and reduced to a lower dimension using **PCA** (Principal Component Analysis) and **t-SNE** (t-Distributed Stochastic Neighbor Embedding). The goal is to identify meaningful customer segments for targeted marketing strategies.
## Requirements
Before running the code, make sure you have Python 3.x and the necessary libraries installed.
### Dependencies:
- `pandas`
- `scikit-learn`
- `matplotlib`
- `seaborn`
You can install all the dependencies by running the following command:
```bash
pip install -r requirements.txt
```
## Project Structure
The project folder structure is as follows:
```
├── data/                   # Folder containing the dataset
│   └── customer_data.csv   # Input customer dataset (replace with your dataset)
├── notebooks/               # Jupyter notebooks (optional)
│   └── segmentation_analysis.ipynb  # Jupyter notebook for step-by-step analysis
├── main.py                  # Main Python script for clustering and analysis
├── requirements.txt         # List of required dependencies
├── README.md                # This file
```

## How to Run the Code

### 1. **Prepare the Data**  
Ensure the dataset (e.g., `customer_segmentation_dataset.xlsx`) is placed in the `data/` folder. You can replace the dataset with your own, ensuring it has the necessary features for clustering (e.g., customer attributes, behavior, etc.).

### 2. **Run the Python Script**
The clustering and analysis can be executed through the `main.py` script. Follow these steps:
1. Open a terminal or command prompt.
2. Navigate to the directory where the project is located.
3. Run the following command:

   ```bash
   python main.py
   ```
The script will:
- Load and preprocess the customer data.
- Apply **PCA** for dimensionality reduction.
- Perform **KMeans clustering** to segment the customers into clusters.
- Use **t-SNE** to visualize the data in 2D and 3D.
- Output the cluster characteristics and suggest personalized marketing strategies.

### 3. **Jupyter Notebook (Optional)**
If you prefer using Jupyter notebooks for step-by-step analysis, you can open the `segmentation_analysis.ipynb` notebook.

To run the notebook:
1. Install Jupyter (if not already installed):

   ```bash
   pip install notebook
   ```

2. Start the notebook server:

   ```bash
   jupyter notebook
   ```

3. Open `segmentation_analysis.ipynb` and run the cells sequentially.

### 4. **Output**
- **2D and 3D Visualizations**: The script generates visualizations using **t-SNE** and **PCA** to illustrate how the clusters are distributed in lower dimensions.
- **Cluster Analysis**: The script prints the average values of features for each cluster, helping identify the characteristics of each customer group.
- **Marketing Recommendations**: Based on the cluster characteristics, the script suggests marketing strategies for each segment, such as targeted offers, loyalty rewards, and premium product promotions.
## Insights & Recommendations
After running the code, you'll receive cluster insights and suggested strategies to engage with each customer segment effectively. Each cluster is characterized by its behavior patterns, and personalized marketing approaches can be derived to maximize customer satisfaction and engagement.
### Suggested Marketing Strategies:
- **Premium Product Engagement**: For clusters with high values in certain features, suggesting premium products can be beneficial.
- **Discount Offers**: Customers responsive to offers or discounts can be targeted with special promotions.
- **Loyalty Programs**: For customers showing loyalty or frequent engagement, loyalty programs and rewards can be implemented to retain them.
## Conclusion
This project demonstrates how machine learning techniques like **KMeans clustering**, combined with dimensionality reduction methods such as **PCA** and **t-SNE**, can uncover hidden patterns in customer behavior. By understanding these patterns, businesses can create effective, personalized marketing strategies to improve engagement, satisfaction, and ultimately sales.
