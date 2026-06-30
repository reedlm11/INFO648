# README: Population Growth Prediction in the Pacific Region

This repository contains a Google Colab notebook that predicts population growth in census tracts within the Pacific Census Division (Alaska, California, Hawaii, Oregon, Washington) for the 2020-2030 decade. The predictions are based on 2010 census characteristics, using machine learning models developed and evaluated through an ablation study.

## How to Run the Notebook

To run this notebook and reproduce the analysis, follow these steps:

1.  **Open in Google Colab**: https://colab.research.google.com/drive/1CGmFmQgyLfjqXXWGZZwzU77kXRzWJPvD#scrollTo=ba70f7e1 and upload the `.ipynb` file from this repository.

2.  **Ensure all data files are present**: The notebook expects these CSV files to be available in the Colab environment:
    *   `student_tracts_raw.csv`: The raw 2010 census data for training and evaluation.
    *   `forecast_tracts_2020.csv`: The 2020 census data used for forecasting 2020-2030 growth.
    *   `data_dictionary.csv`: A dictionary explaining the features in the datasets.

    If these files are not already in your Colab environment, you will need to upload them. You can typically do this by clicking the folder icon on the left sidebar, then the upload icon.

3.  **Run all cells**: Go to `Runtime` -> `Run all` in the Colab menu. The notebook will execute sequentially, performing data loading, preprocessing, model training, evaluation, and forecasting.

4.  **Review the output**: The notebook is structured with markdown cells explaining each phase of the analysis, along with visualizations and model performance metrics. The final section provides the 2020-2030 growth predictions and recommendations.

## Data Sources

*   **2010 Census Data**: Demographic, housing, and geographic characteristics of census tracts in the Pacific region, used for training the predictive models and defining the target variable (2010-2020 population growth).
*   **2020 Census Data (Interpolated)**: Demographic, housing, and geographic characteristics for census tracts in 2020. This data was used to forecast population growth for the 2020-2030 period. Note that 2020 population figures were interpolated where necessary.

All data is at the census tract level for the Pacific Census Division, which includes Alaska, California, Hawaii, Oregon, and Washington.
