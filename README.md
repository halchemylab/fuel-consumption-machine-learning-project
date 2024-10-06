# Fuel Consumption Prediction API

This is a FastAPI-based API that provides fuel consumption predictions using a trained linear regression model. The API is built using Python and uses the following libraries:

- FastAPI
- Pydantic
- joblib

## Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/fuel-consumption-prediction-api.git
```

2. Navigate to the project directory:

```bash
cd fuel-consumption-prediction-api
```

3. Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Usage

1. Train the model:

```bash
python analysis.ipynb
```

2. Start the FastAPI server:

```bash
uvicorn app:app --reload
```

3. Make a prediction request:

```bash
curl -X POST http://localhost:8000/predict/ -H 'Content-Type: application/json' -d '{"input1": 2.0, "input2": 4.0}'
```

## Data

The data used for training the model is available in the `data` directory. The data is a CSV file containing fuel consumption data for various vehicles.

dataset_source = "https://www.kaggle.com/datasets/krupadharamshi/fuelconsumption"

## Model

The model used in this API is a linear regression model trained on the fuel consumption data. The model is exported as a pickle file (`linear_model.pkl`) in the `models` directory.

## Contact

If you have any questions or issues, please contact the project maintainer at hyp243@nyu.edu (mailto:hyp243@nyu.edu).

I hope this helps! Let me know if you have any other questions.
