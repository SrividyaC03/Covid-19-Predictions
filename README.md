# Covid-19-Predictions using ML
### Project Overview
This project focuses on analyzing global COVID-19 data to uncover insights into the virus spread and predict future trajectories using machine learning techniques. The analysis aims to utilize various statistical and machine learning models to assess the impact of quarantine measures and forecast important outcomes like infection rates and recovery chances.

### Dataset
The dataset used in this project comprises daily updates on COVID-19 statistics from around the world, including infection rates, recoveries, and death tolls. The data is sourced from publicly available records maintained by health organizations.

### Features
- Date: The date on which the data was recorded.
- Province/State: Sub-national division detailing the location.
- Country/Region: The country or region of the data.
- Latitude and Longitude: Geographical coordinates.
- Confirmed Cases: Total number of confirmed COVID-19 cases.
- Deaths: Total number of deaths due to COVID-19.  
- Recovered: Total number of recovered patients.
- Active Cases: Current active COVID-19 cases.
- WHO Region: WHO regional classifications to analyze regional responses.

### Technologies Used
- Python: For scripting and analysis.
- Pandas & NumPy: For data manipulation and cleaning.
- Scikit-Learn: For implementing machine learning models.
- Matplotlib & Seaborn: For data visualization.
- Jupyter Notebook: For interactive code execution and visualization.

### Project Workflow
1. Data Extraction

      The data extraction phase begins by loading the COVID-19 dataset, which includes daily statistics on confirmed cases, deaths, recoveries, and active cases from countries around the world. The dataset consists of 49,069 entries with 10 columns, each providing specific insights into the pandemic's global spread.

2. Data Transformation
      In this phase, the following steps are executed to prepare the data for analysis:

      - Data Cleaning: Handle missing values, especially in the 'Province/State' column, and remove duplicate entries.
      - Data Type Conversion: Convert the 'Date' column to datetime format for time-series analysis.
      - Feature Engineering: Calculate additional metrics like the Case Fatality Rate and Recovery Rate, and filter out rows with zero confirmed cases to focus on meaningful data.

3. Exploratory Data Analysis (EDA)
   - Loading and Preliminary Examination: Use Pandas to load the dataset and inspect the first few entries to understand its structure.
   - Visual Analysis: Employ Matplotlib and Seaborn for creating visualizations such as global scatter plots of confirmed cases and time-series plots of cases over time.
   - Statistical Analysis: Generate descriptive statistics to understand data distribution and identify outliers.
4. Model Building

     Two main models are employed:
   - Random Forest Regressor: This model is used for its effectiveness in handling non-linear data and its ability to perform feature importance analysis.
   - Support Vector Machine (SVM): Chosen for its capability to manage high-dimensional spaces through kernel methods.

5. Model Evaluation
  - Performance Metrics: Evaluate model performance using Mean Squared Error (MSE) and R² scores.
  - Feature Importance: Analyze the contribution of each feature to the model predictions.
  - Classification Analysis: For binary outcomes (recovery vs. death), use F1-score and confusion matrices to assess model precision and recall.

6. ETL Process Completion

    After transformation and analysis, the clean, processed data is saved to a CSV file, ensuring that it can be easily accessed for future analyses without the need to repeat preprocessing steps.

7. Results and Model Insights
  - Model Comparisons: Contrast the performance and feature importance of the Random Forest and SVM models.
  - Outcome Predictions: Utilize the models to predict and classify the outcomes of COVID-19 cases based on the severity and spread within regions.

### Future Improvements
- Incorporate More Data: As more data becomes available, including newer variants and vaccine data.
- Enhance Models: Refine models with additional tuning and explore ensemble methods for better accuracy.
- Real-Time Analysis: Develop capabilities for real-time data analysis and prediction.

### Contributions

Contributions are welcome. Please fork the repository and create a pull request with your proposed updations.
