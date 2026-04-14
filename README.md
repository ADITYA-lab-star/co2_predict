# CO2 Emission Prediction Using Machine Learning

## Overview

This project is a web-based application that predicts CO2 emissions of vehicles based on their engine size using a machine learning model. Built with Flask and scikit-learn, it provides a simple interface for users to input engine size and receive an estimated CO2 emission value.

The prediction model is trained on a dataset containing various vehicle attributes and their corresponding CO2 emissions. The application demonstrates the practical application of machine learning in environmental analysis.

## Features

- **Web Interface**: User-friendly web application built with Flask
- **Machine Learning Prediction**: Utilizes a trained regression model to predict CO2 emissions
- **Real-time Results**: Instant prediction results displayed on the web page
- **Dataset Analysis**: Based on comprehensive vehicle fuel consumption data

## Dataset

The project uses the `FuelConsumptionCo2.csv` dataset, which contains the following columns:
- MODELYEAR: Model year of the vehicle
- MAKE: Vehicle manufacturer
- MODEL: Specific model name
- VEHICLECLASS: Class of the vehicle (e.g., COMPACT, SUV - SMALL)
- ENGINESIZE: Engine size in liters
- CYLINDERS: Number of cylinders
- TRANSMISSION: Type of transmission
- FUELTYPE: Type of fuel used
- FUELCONSUMPTION_CITY: Fuel consumption in city (L/100 km)
- FUELCONSUMPTION_HWY: Fuel consumption on highway (L/100 km)
- FUELCONSUMPTION_COMB: Combined fuel consumption (L/100 km)
- FUELCONSUMPTION_COMB_MPG: Combined fuel consumption in MPG
- CO2EMISSIONS: CO2 emissions in grams per km

## Installation

### Prerequisites

- Python 3.7 or higher
- pip (Python package manager)

### Steps

1. **Clone the repository** (if applicable) or navigate to the project directory:
   ```
   cd Co2-Emission-Prediction-Using-Machine-Learning
   ```

2. **Install required packages**:
   ```
   pip install flask scikit-learn pandas numpy
   ```

3. **Ensure the model file is present**:
   - The application requires `model.pkl`, which should be a trained machine learning model.
   - If not present, you may need to train the model using the provided dataset.

4. **Set up templates** (if missing):
   - The application expects `templates/index.html` and `templates/result.html`.
   - Create these HTML files for the web interface.

## Usage

1. **Run the application**:
   ```
   python main.py
   ```

2. **Access the web interface**:
   - Open a web browser and navigate to `http://127.0.0.1:5000/`

3. **Make predictions**:
   - Enter the engine size (in liters) in the input field
   - Submit the form to get the predicted CO2 emissions

## Model Details

- **Algorithm**: The model uses a regression algorithm (likely Linear Regression or similar) trained on the FuelConsumptionCo2 dataset
- **Input Feature**: Engine size (ENGINESIZE)
- **Output**: Predicted CO2 emissions in grams per km
- **Training Data**: Historical vehicle data with various attributes

## Project Structure

```
Co2-Emission-Prediction-Using-Machine-Learning/
├── main.py                 # Flask application
├── model.pkl              # Trained machine learning model
├── FuelConsumptionCo2.csv # Dataset
├── templates/
│   ├── index.html         # Main page template
│   └── result.html        # Results page template
└── README.md              # This file
```

## Dependencies

- Flask: Web framework for Python
- scikit-learn: Machine learning library
- pandas: Data manipulation library
- numpy: Numerical computing library

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- Dataset source: Original fuel consumption data
- Built as a demonstration of machine learning applications in environmental science
