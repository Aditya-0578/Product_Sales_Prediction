# Product Sales Prediction

This repository contains a complete machine learning pipeline in Jupyter Notebook for predicting product sales based on historical supermarket data. The project demonstrates data preprocessing, exploratory data analysis (EDA), feature engineering, model building, and evaluation.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Results & Conclusion](#results--conclusion)
- [Contributing](#contributing)
- [License](#license)

## Overview

The goal of this project is to estimate product sales using machine learning techniques. By analyzing various attributes like product type, store characteristics, and pricing, the model aims to provide accurate sales predictions that can help businesses optimize inventory and marketing strategies.

## Dataset

- **File:** Sales.csv
- **Description:** This dataset contains historical sales records for various products across multiple outlets.
- **Features include:**
  - `Item_Identifier`: Unique ID for each product
  - `Item_Weight`: Weight of the product
  - `Item_Fat_Content`: Fat content of product
  - `Item_Visibility`: Percentage of total display area of all products in a store allocated to the product
  - `Item_Type`: Category of product (Dairy, Soft Drinks, Meat, etc.)
  - `Item_MRP`: Maximum Retail Price
  - `Outlet_Identifier`: Store ID
  - `Outlet_Establishment_Year`: Year store was established
  - `Outlet_Size`: Store size (Small/Medium/High)
  - `Outlet_Location_Type`: Tier of city
  - `Outlet_Type`: Store type (Grocery Store, Supermarket Type1, etc.)
  - `Item_Outlet_Sales`: Sales of the product in a particular store (target variable)

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Aditya-0578/Product_Sales_Prediction.git
   cd Product_Sales_Prediction
   ```

2. **Install required packages:**
   You can use the following command, or install packages individually if a requirements.txt is not provided:
   ```bash
   pip install numpy pandas scikit-learn matplotlib seaborn jupyter
   ```

## Usage

1. **Dataset:** Ensure `Sales.csv` is present in the project directory.
2. **Notebook:** Open the main notebook:
   ```bash
   jupyter notebook MarketSalesPredictor.ipynb
   ```
3. **Run the notebook:** Execute each cell step by step to:
   - Load and preprocess the data
   - Perform EDA and visualize trends
   - Build and evaluate machine learning models for sales prediction

## Project Structure

```
Product_Sales_Prediction/
│
├── MarketSalesPredictor.ipynb  # Main notebook with full workflow
├── Sales.csv                   # Dataset
├── README.md                   # Project documentation
└── requirements.txt            # (Optional) Python dependencies
```

## Results & Conclusion

- The notebook explores several regression models to predict `Item_Outlet_Sales`.
- Key steps include handling missing data, encoding categorical variables, and feature engineering.
- Model performance is evaluated using metrics such as RMSE (Root Mean Squared Error).
- Visualizations and comparison of model results are included within the notebook.
- **Conclusion:** The machine learning model effectively predicts product sales based on the provided features. Insights from EDA can help businesses understand which factors most influence sales, guiding better decision-making.

## Contributing

Contributions are welcome! If you'd like to improve this project, please fork the repository and submit a pull request. For major changes, open an issue first to discuss your ideas.

## License

This project is open source and available under the [MIT License](LICENSE).
