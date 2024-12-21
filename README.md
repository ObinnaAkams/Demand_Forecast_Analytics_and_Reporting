# Demand Forecast Analytics and Reporting

## Overview
This repository contains two key components:
1. A Jupyter Notebook (`Model_Notebook.ipynb`) for data preprocessing, analysis, and forecasting.
2. A Power BI report (`PVM_Report.pbix`) visualizing insights derived from the notebook's analysis.

The project focuses on analyzing and forecasting production volumes for Perfetti Van Melle, incorporating assumptions about data grouping and addressing regional variations.

## File Descriptions

### 1. Model_Notebook.ipynb
#### Purpose
The notebook serves as a pipeline for:
- Data preprocessing and cleaning.
- Extracting top-performing SKUs by region.
- Developing and evaluating forecasting models for production volumes.

#### Key Sections
1. **Library Imports**:
   - Includes Python libraries like `pandas`, `numpy`, `matplotlib`, `seaborn`, and `scikit-learn`.
   - Required for data manipulation, visualization, and machine learning.

2. **Data Processing**:
   - Function `extract_top_sku_by_region`: Extracts the top 5 SKUs per region from Excel files.
   - Function `load_and_process_data`: Reads CSV data, processes date columns, and renames fields for consistency.

3. **Forecasting Model**:
   - A predictive model is developed to forecast production volumes based on historical data.
   - Utilizes linear regression and polynomial features for performance enhancement.

4. **Output and Integration**:
   - The results from the notebook are intended for integration into Power BI visualizations.

### 2. PVM_Report.pbix
#### Purpose
The Power BI report visualizes:
- Production volume trends across regions.
- Top-performing SKUs and their distribution.
- Forecasts for future production volumes.

#### Notes
Ensure the data processed in the notebook is loaded into Power BI for accurate visualizations. Specific measures and dimensions used in the report can be customized based on business needs.

## Setup Instructions

### Prerequisites
1. Python 3.7 or higher.
2. Jupyter Notebook installed (via `pip install notebook`).
3. Power BI Desktop for opening `.pbix` files.

### Python Dependencies
Install the required Python libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Running the Notebook
1. Open the notebook:
   ```bash
   jupyter notebook Model_Notebook.ipynb
   ```
2. Follow the instructions within each cell to execute the preprocessing and modeling steps.
3. Export the processed data as needed for Power BI.

### Using the Power BI Report
1. Open `PVM_Report.pbix` in Power BI Desktop.
2. Load the processed data from the notebook into Power BI.
3. Explore and customize the visualizations as needed.

## Outputs

### Notebook
- Cleaned datasets ready for visualization.
- Forecasting model outputs and performance metrics.

### Power BI Report
- Interactive dashboards showcasing production trends, SKU performance, and forecasts.

## Assumptions and Considerations
- **Data Units**: Production volume is measured in tonnes.
- **Region Grouping**: Regions not explicitly defined are grouped as "OTHERS."
- **Data Sources**: Ensure data is consistent and updated for accurate analysis and reporting.


