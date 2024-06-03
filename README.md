# Census Analysis and Prediction

This repository contains a project for analyzing and predicting population trends using Long Short-Term Memory (LSTM) neural networks. The project focuses on population data from China and Kenya.

## Project Overview

The goal of this project is to analyze historical population data and build an LSTM model to forecast future population trends. The project includes the following steps:
1. Data preprocessing
2. Creating sequences for LSTM
3. Building and training the LSTM model
4. Evaluating the model
5. Visualizing the results
6. Analyzing the trends and patterns

## Dependencies

- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- TensorFlow
- Keras

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/Census-Analysis-and-Prediction.git
    cd Census-Analysis-and-Prediction
    ```

2. Install the required packages:
    ```bash
    pip install numpy pandas matplotlib scikit-learn tensorflow keras
    ```

## Data

The dataset includes historical population data for China and Kenya. Ensure your data is saved as `china.csv` and `kenya.csv` in the root directory of this project.

## Usage

1. Prepare your data and save it as `china.csv` and `kenya.csv`.
2. Run the script to preprocess the data, build the model, and visualize the results:
    ```bash
    python population_forecasting.py
    ```

## Analysis

### Data Overview
The dataset includes the following columns:
- `Year`: The year of the data record.
- `Population`: Total population.
- `Urban Population`: Urban population.
- `Rural Population`: Rural population.
- `Male Population`: Male population.
- `Female Population`: Female population.
- `Birth Rate`: Birth rate per 1000 people.
- `Death Rate`: Death rate per 1000 people.
- `Life Expectancy`: Life expectancy in years.

### Data Preprocessing
- Normalization: The population data is normalized to a range between 0 and 1 using Min-Max scaling.
- Splitting: The dataset is split into training and testing sets with an 80-20 ratio.
- Sequence Creation: Data is converted into sequences with a specified number of time steps to be used as input features for the LSTM model.

### Model Building
- An LSTM model is constructed using TensorFlow Keras with the following layers:
  - LSTM layer with 50 units
  - Dense layer with 1 unit

### Training and Evaluation
- The model is trained with the training data and validated with the testing data over 100 epochs.
- Loss curves for training and validation data are plotted to visualize model performance.

### Results
- Predictions are made on the training and testing data.
- The actual vs. predicted population trends are plotted to evaluate the model's performance.

## Results

The model's performance is displayed through:
1. Training and validation loss plots.
2. Actual vs. predicted population trends.

## Contributing

Feel free to open issues or submit pull requests for any improvements or bug fixes.

## License

This project is licensed under the MIT License.
