
# Customer Segmentation Project

## Overview

This project aims to perform customer segmentation using various clustering algorithms. By segmenting customers into different groups based on their purchasing behavior, businesses can tailor marketing strategies to improve customer engagement, retention, and overall sales.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Methodology](#methodology)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Dataset

The project utilizes three main datasets:

1. `List_of_Orders`:
   - `Order ID`
   - `Order Date`
   - `CustomerName`
   - `State`
   - `City`

2. `Order_Details`:
   - `Order ID`
   - `Amount`
   - `Profit`
   - `Quantity`
   - `Category`
   - `Sub-Category`

3. `Sales_Target`:
   - `Month of Order Date`
   - `Category`
   - `Target`

## Project Structure

```
customer-segmentation/
├── data/
│   ├── list_of_orders.csv
│   ├── order_details.csv
│   └── sales_target.csv
├── notebooks/
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_exploratory_data_analysis.ipynb
│   ├── 03_feature_engineering.ipynb
│   └── 04_clustering_and_evaluation.ipynb
├── src/
│   ├── data_preprocessing.py
│   ├── exploratory_data_analysis.py
│   ├── feature_engineering.py
│   └── clustering.py
├── results/
│   ├── cluster_profiles.csv
│   └── cluster_visualizations.png
├── README.md
└── requirements.txt
```

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Ragulvasan08/customer-segmentation.git
   ```

2. Navigate to the project directory:

   ```bash
   cd customer-segmentation
   ```

3. Create and activate a virtual environment (optional but recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

4. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Data Preprocessing and Cleaning:
   - Run the `01_data_preprocessing.ipynb` notebook to load, clean, and preprocess the data.

2. Exploratory Data Analysis (EDA):
   - Run the `02_exploratory_data_analysis.ipynb` notebook to perform EDA and understand the data distributions and patterns.

3. Feature Engineering:
   - Run the `03_feature_engineering.ipynb` notebook to create and standardize features for clustering.

4. Clustering and Evaluation:
   - Run the `04_clustering_and_evaluation.ipynb` notebook to apply clustering algorithms and evaluate the clusters.

## Methodology

The project follows these steps:

1. Data Ingestion & Merging:
   - Load datasets and merge `List_of_Orders` and `Order_Details`.

2. Data Preprocessing & Cleaning:
   - Handle missing values, remove duplicates, and convert date columns to datetime format.

3. Exploratory Data Analysis (EDA):
   - Analyze data distributions, identify patterns, and visualize key statistics.

4. Feature Engineering:
   - Create RFM (Recency, Frequency, Monetary) features and standardize them.

5. Clustering Algorithms:
   - Apply K-Means, DBSCAN, and Agglomerative Clustering to segment customers.

6. Evaluating and Interpreting Clusters:
   - Calculate mean values of RFM features for each cluster, create cluster profiles, and visualize clusters.

7. Actionable Insights and Recommendations:
   - Derive insights for tailored marketing strategies and recommendations to improve customer engagement and retention.

## Results

- K-Means Silhouette Score: 0.36198777701488555
- Detailed cluster profiles and visualizations are saved in the `results/` directory.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or new features.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any questions or suggestions, please contact RAGUL.S - ragzvaz08@gmail.com.
