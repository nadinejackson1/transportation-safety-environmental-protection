# Transportation Safety Environmental Protection Analysis (10-Year Overview)
🚂 ⚠️ Analyzing data on train derailments in the context of transportation safety and environmental protection. This project aims to analyze train accident causes over the last 10 years, focusing on hazmat releases and hazmat cars damaged/derailed incidents. The dataset used in this analysis is a table called "10-year Accident/Incident Overview by Calendar Year," which provides a comprehensive view of various train accident-related parameters.🚂 ⚠️

### Dataset

The dataset is an Excel file (10yearrailroadaccidentincidentoverview.xlsx) that contains information on train accidents and incidents from 2014 to 2023. I excluded the year 2023 because it is the current year and only partial data is available, which was schuewing the prediction. The dataset was gathered from the Federal Railroad Administration, Office of Safety Analysis at https://safetydata.fra.dot.gov/officeofsafety/publicsite/query/TenYearAccidentIncidentOverview.aspx 

The columns used in the dataset are:

    Category
    CY 2014
    CY 2015
    CY 2016
    CY 2017
    CY 2018
    CY 2019
    CY 2020
    CY 2021
    CY 2022

The rows under the 'Category' column used include:

    --- HAZMAT RELEASES
    --- Cars carrying hazmat
    --- Hazmat cars damaged/derailed
    TOTAL ACCIDENTS/INCIDENTS

### Methodology

We have used Python with Pandas, NumPy, and scikit-learn libraries to preprocess the data, train machine learning models, and make predictions. We have created separate Linear Regression models to predict the number of hazmat releases and hazmat cars damaged/derailed incidents based on the year.

### Getting Started

    Clone this repository.
    Ensure you have Python 3.x installed.
    Install the required packages: pandas, numpy, scikit-learn, and openpyxl (for reading Excel files).


pip install pandas numpy scikit-learn openpyxl

    Run the Jupyter Notebook or the Python script to see the analysis and predictions.

### Results

The trained Linear Regression models predict the number of hazmat releases and hazmat cars damaged/derailed incidents for a given year. The performance of the models can be evaluated using mean squared error and R-squared scores. Depending on the use case and data complexity, other machine learning models can be explored to improve prediction accuracy.
Contributing

Contributions are welcome! If you'd like to improve the analysis or explore different machine learning models, please feel free to create a pull request or open an issue.
License

This project is open-source and available under the MIT License.
