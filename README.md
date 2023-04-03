# Transportation Safety Environmental Protection Analysis 
🚂 ⚠️ Analyzing data on train derailments in the context of transportation safety and environmental protection. This repository contains a Python implementation of a linear regression model to predict the number of hazmat releases and hazmat cars damaged/derailed per year, using a dataset containing 9 years of railway accident/incident data. Additionally, the model takes into account the ratio of hazmat cars damaged/derailed to total accidents as a feature🚂 ⚠️

🌟I have learned more with trial and error on this project than I initially intended. After receiving results I wasn't happy with on the Linear Regression Model, I tried Random Forest Regressor and then Gradient Boosting Regressor. Although the model for HAZMAT RELEASES prediction improved significantly with hyperparameter tuning, the model for Hazmat cars damaged/derailed prediction did not improve. So I went back to Linear Regression and added an additional feature calculating the ratio of hazmat cars damaged/derailed to total accidents with hopes that it would help my small dataset.

***This is my first public project that wasn't a school/training related project and I am very passionate about it! Contributions are welcome! If you'd like to improve the analysis or explore different machine learning models, please feel free to create a pull request or open an issue. Thank you!***

### Dataset

The dataset is an Excel file (10yearrailroadaccidentincidentoverview.xlsx) that contains information on train accidents and incidents from 2014 to 2023. I excluded the year 2023 because it is the current year and only partial data is available, which was skewing the prediction. The dataset was gathered from the Federal Railroad Administration, Office of Safety Analysis at https://safetydata.fra.dot.gov/officeofsafety/publicsite/query/TenYearAccidentIncidentOverview.aspx 

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

### Dependencies

This project requires the following Python libraries:

    pandas
    numpy
    scikit-learn
    openpyxl (for reading Excel files)

You can install these libraries using pip:

    pip install pandas numpy scikit-learn openpyxl

### Usage

Clone this repository:

    git clone https://github.com/yourusername/railway-hazmat-accident-prediction.git
    cd railway-hazmat-accident-prediction

Place the 10yearrailroadaccidentincidentoverview.xlsx file in the project folder.

Run the main.py script to preprocess the data, train the linear regression model, and evaluate the model's performance:

    python main.py

To make predictions for specific years, modify the years_to_predict list in the main.py script and run the script again. The script will print the predicted number of hazmat releases and hazmat cars damaged/derailed for the specified years.

## Note

The performance of the current model may not be very good due to the small dataset size and the nature of the problem. To improve the model's performance, you can try gathering more data, using other features, or experimenting with different machine learning algorithms.

### License

This project is licensed under the MIT License. See the LICENSE file for details.

### Methodology

I used Python with Pandas, NumPy, and scikit-learn libraries to preprocess the data, train machine learning models, and make predictions. We have created separate Linear Regression models to predict the number of hazmat releases and hazmat cars damaged/derailed incidents based on the year.

### Getting Started

    Clone this repository.
    Ensure you have Python 3.x installed.
    Install the required packages: pandas, numpy, scikit-learn, and openpyxl (for reading Excel files).


pip install pandas numpy scikit-learn openpyxl

    Run the Jupyter Notebook or the Python script to see the analysis and predictions.

### Results

The trained Linear Regression models predict the number of hazmat releases and hazmat cars damaged/derailed incidents for a given year. The performance of the models can be evaluated using mean squared error and R-squared scores. Depending on the use case and data complexity, other machine learning models can be explored to improve prediction accuracy.

### Contributing

Contributions are welcome! If you'd like to improve the analysis or explore different machine learning models, please feel free to create a pull request or open an issue.

### License

This project is open-source and available under the MIT License.
