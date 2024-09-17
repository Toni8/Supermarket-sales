# Supermarket Sales Analysis and Prediction

## Project Overview
This project presents a comprehensive analysis of supermarket sales data across three branches over a three-month period. Utilizing a combination of data cleaning, visualization, and predictive modeling techniques, we aim to uncover valuable insights and forecast future sales trends in a competitive market environment.

## Tools and Technologies
- **MySQL**: Used for data cleaning and preparation of the original dataset.
- **Microsoft Power BI**: Employed for creating interactive dashboards and visualizations.
- **Python**: Used for predictive modeling of sales peaks.

## Data Source
The dataset includes sales information from three branches of a supermarket chain, covering various aspects such as:
- Customer types
- Product lines
- Branch-specific performance
- Daily sales figures

## Project Phases

### 1. Data Cleaning and Preparation (MySQL)
- Cleaned and structured the raw data.
- Created views for different analysis perspectives, including the `time_based_analysis` view for time series analysis.

### 2. Data Visualization (Power BI)
Created interactive dashboards showcasing:
- Time-based sales trends
- Customer segmentation analysis
- Product line performance
- Branch-wise comparisons

### 3. Predictive Modeling (Planned)
- Will use the `time_based_analysis` dataset to build a model for predicting peak sales dates.
- Techniques used: Machine Learning algorithms suitable for time-series prediction.

## Key Insights
1. **Branch Performance**: Comparative analysis of sales and efficiency across three branches.
2. **Product Trends**: Identification of top-performing product lines and customer preferences.
3. **Customer Behavior**: Analysis of purchasing patterns between member and non-member customers.
4. **Temporal Patterns**: Recognition of daily, weekly, and monthly sales trends.


## How to Use This Repository

1. **Data**: The cleaned datasets and SQL views are available in the `data` folder.
2. **Visualizations**: Power BI dashboard files can be found in the `powerbi` folder.
3. **Documentation**: Detailed analysis reports and insights are in the `docs` folder.
4. **Scripts**: 
   - SQL scripts used for data cleaning are in the `sql_scripts` folder.
   - A Python notebook (`predictive_model.ipynb`) for building and training the sales prediction model is located in the `python_scripts` folder.
5. **Models**: Trained machine learning models will be saved in the `models` folder inside the `python_scripts` folder..

To run the predictive model:
1. Ensure you have Python installed with necessary libraries (requirements listed in `requirements.txt`).
2. Open the `predictive_model.ipynb` notebook in Jupyter or your preferred Python IDE.
3. Follow the step-by-step instructions in the notebook to load data, train the model, and make predictions.



## License
This project is licensed under the MIT License - see the `LICENSE.md` file for details.

## Acknowledgments
- Thanks to [Data Source Provider] for the initial dataset.
- Appreciation to the open-source community for the tools and libraries used in this project.
