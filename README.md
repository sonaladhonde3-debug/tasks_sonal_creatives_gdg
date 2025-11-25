# Task 1 - Crab Age Analysis & EDA

This branch contains all files related to the Crab Age Analysis task.

## Files Included
- `SONAL_Task1.ipynb` – The Colab notebook containing the complete EDA, feature engineering, and preprocessing pipeline.
- `Task1_crabs.csv` – The dataset containing physical measurements of crabs.
- `README.md` – Explanation of the task, workflow, and findings.

## Task Description
This task involves a detailed Exploratory Data Analysis (EDA) and preprocessing pipeline to understand patterns in crab physical attributes and their relation to age.

**Technologies Used:**
- Python 3, Pandas, NumPy
- Matplotlib & Seaborn (Visualization)
- YData Profiling (Automated Reporting)
- Scikit-learn (Preprocessing)

**Workflow Overview:**
- **Data Loading & Cleaning**: Loaded the dataset, removed non-predictive columns (e.g., `id`), and handled null values.
- **Exploratory Data Analysis (EDA)**:
    - Generated automated profile reports.
    - Created visualizations including Bar Charts (Sex balance), Box Plots (Age spread), KDE Plots (Density), and Violin Plots.
    - Analyzed correlations using Heatmaps.
- **Feature Engineering**:
    - Applied One-Hot Encoding to the `Sex` column.
    - Created a new feature `Lost Weight` to analyze measurement discrepancies.
- **Standardization**: Applied Standard Scaling (Z-score normalization) to numerical columns for machine learning readiness.

## How to Run
1. **Prerequisites**: Install the required libraries by running:
   `pip install pandas numpy matplotlib seaborn ydata-profiling scikit-learn`
2. **Launch**: Open the `SONAL_Task1.ipynb` notebook in Google Colab.
3. **Data Setup**: Upload `Task1_crabs.csv` and update the file path in the data loading cell if necessary.
4. **Execution**: Run the cells sequentially to generate the analysis and visualizations.

## Results
- **Correlations**: `Shell Weight` showed the highest correlation with `Age` (approx. 0.66), making it the strongest predictor.
- **Physical Dimensions**: Features like `Height`, `Diameter`, and `Length` exhibited moderate positive correlations with age.
- **Feature Importance**: The derived `Lost Weight` feature had a low correlation (0.15), suggesting it is less predictive than raw weight metrics.
