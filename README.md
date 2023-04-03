# Transportation Safety Environmental Protection Analysis 
🚂💭 Analyzing data on train derailments in the context of transportation safety and environmental protection. This repository contains a Python script that uses machine learning models to predict the number of Hazmat releases and Hazmat cars damaged/derailed in a given year based on historical railroad accident and incident data. The data covers a 39-year period and is analyzed using Linear Regression, Random Forest, and Gradient Boosting models.

🌟Throughout this project, I've learned more with trial and error than I initially intended. After receiving unsatisfactory results from the Linear Regression Model, I tried Random Forest Regressor and then Gradient Boosting Regressor. The performance of the models varied, with the Gradient Boosting model performing the best for predicting Hazmat Releases and the Linear Regression model performing the best for predicting Hazmat Cars Damaged/Derailed based on their mean RMSE scores from cross-validation.

***This is my first public project that wasn't a school/training related project and I am very passionate about it! Contributions are welcome! If you'd like to improve the analysis or explore different machine learning models, please feel free to create a pull request or open an issue. Thank you!***

### Dataset

The dataset is an Excel file (39yearrailroadaccidentincidentoverview.xlsx) that contains information on train accidents and incidents from 1984 to 2022. I excluded the year 2023 because it is the current year and only partial data is available, which was skewing the prediction. The dataset was gathered from the Federal Railroad Administration, Office of Safety Analysis at https://safetydata.fra.dot.gov/officeofsafety/publicsite/query/TenYearAccidentIncidentOverview.aspx 

### Requirements

    Python 3.x
    pandas
    numpy
    scikit-learn
    openpyxl (for reading Excel files)

### Installation

1. Clone this repository.
2. Ensure you have Python 3.x installed.
3. Install the required packages: pandas, numpy, scikit-learn, and openpyxl (for reading Excel files).

### Usage

Run the script to see the analysis and predictions. The script will train and evaluate Linear Regression, Random Forest, and Gradient Boosting models for predicting the number of Hazmat releases and Hazmat cars damaged/derailed incidents. Evaluation metrics include mean squared error (MSE), root mean squared error (RMSE), mean absolute error (MAE), and R-squared (R²) scores.

Cross-validation is also used to further evaluate model performance. Based on the cross-validation results, the script will suggest the best model for predicting Hazmat releases and Hazmat cars damaged/derailed incidents.

### Results

The script provides predictions for the number of Hazmat releases and Hazmat cars damaged/derailed incidents for a specific year. The performance of the models can be evaluated using the mean squared error, mean absolute error, R-squared scores, and cross-validation. Depending on the use case and data complexity, other machine learning models can be explored to improve prediction accuracy.

## Note

The performance of the current model may not be very good due to the small dataset size and the nature of the problem. To improve the model's performance, you can try gathering more data, using other features, or experimenting with different machine learning algorithms.

### Contributing

Contributions are welcome! If you'd like to improve the analysis or explore different machine learning models, please feel free to create a pull request or open an issue.

### License

This project is open-source and available under the MIT License.
