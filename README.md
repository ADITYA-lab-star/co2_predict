
# 🌍 CO2 Emission Predictor

## 📌 Overview
The **CO2 Emission Predictor** is an applied machine learning regression project designed to analyze historical environmental datasets and forecast future CO2 emissions. This project features a trained model deployable via a simple web application, aiming to provide actionable insights for organizations and policymakers to implement effective climate strategies.

The model achieves an **85% prediction accuracy** through robust feature engineering and optimized regression algorithms.

## 🚀 Features
* **Predictive Modeling:** Implementation of regression algorithms, including Random Forest Regressor and Linear Regression.
* **Web Deployment:** A functional web interface for real-time model interaction.
* **Performance Evaluation:** Rigorous testing using standard metrics (RMSE, R-squared) to ensure high-fidelity forecasting.

## 🛠️ Tech Stack
* **Language:** Python
* **Web Framework:** Flask
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-learn
* **Model Serialization:** Joblib (used for `model.pkl`)

## 📂 Project Structure
```text
co2_predict/
├── templates/              # HTML templates for the web application
│   ├── index.html          # Main landing and input page
│   └── result.html         # Page to display prediction results
├── FuelConsumptionCo2.csv # The raw dataset used for training
├── README.md               # Project documentation (this file)
├── main.py                # Main web application entry point (Flask app)
├── model.pkl               # The trained machine learning model file
├── train.py                # Script to (re)train the model
└── requirements.txt        # Project dependencies
````

## ⚙️ Installation & Setup

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/ADITYA-lab-star/co2_predict.git](https://github.com/ADITYA-lab-star/co2_predict.git)
    cd co2_predict
    ```

2.  **Create a virtual environment (Recommended):**

    ```bash
    python -m venv env
    source env/bin/activate  # On Windows use: env\Scripts\activate
    ```

3.  **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

## 📊 Usage

### To run the trained model as a web application:

Run the main script:

```bash
python main.py
```

Open your web browser and navigate to the application's local address (e.g., `http://127.0.0.1:5000/`). You can then enter vehicle parameters and view predicted CO2 emissions.

### To re-train the model:

If you wish to re-train the model with new data or a new algorithm:

```bash
python train.py
```

This script will produce a new `model.pkl` file, which `main.py` will use on the next run.

## 📈 Model Performance

  * **Algorithms Tested:** Linear Regression, Random Forest Regressor.
  * **Key Metrics:** Achieved an R-squared / Prediction Accuracy of **\~85%** on the validation set, demonstrating strong generalization on unseen environmental data.

<!-- end list -->
