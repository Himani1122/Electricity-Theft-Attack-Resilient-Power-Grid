# Energy Theft Detection Project

## 1. Project Overview
This project aims to detect energy theft (such as meter tampering or unmetered connections) using machine learning techniques. It leverages historical electricity consumption data to identify anomalous patterns that may indicate fraudulent activity, ultimately helping utility companies reduce non-technical losses.

## 2. Key Features
*   **Data Preprocessing:** Cleans and normalizes raw electricity consumption data.
*   **Feature Engineering:** Extracts relevant features to improve model accuracy.
*   **Machine Learning Model:** Utilizes a trained neural network (or specified ML model) for classification.
*   **Detection System:** Processes input data and outputs a prediction of whether energy theft has occurred.

## 3. Repository Structure
*   `Dataset/`: Contains the dataset and related files.
    *   `datasetlink.txt`: Link to the dataset used for training/testing.
    *   `ElectricityTheft.csv`: Main dataset file.
    *   `test.csv`: Dataset used for testing the model.
*   `model/`: Contains the saved machine learning model.
    *   `model.json`: Model architecture.
    *   `model_weights.h5`: Trained model weights.
*   `ElectricityTheftDetection.py`: The main script for energy theft detection.
*   `run.bat`: Batch file to execute the project.
*   `test.py`: Script for testing the model.

## 4. Prerequisites
Before running the project, ensure you have the following installed:
*   Python 3.x
*   Required Python libraries (e.g., pandas, numpy, tensorflow/keras, scikit-learn).  It is recommended to use a virtual environment.

## 5. Installation and Setup
1.  **Clone the repository:**
    ```bash
    git clone [repository_url]
    cd EnergyTheft
    ```
2.  **Install dependencies:**
    You can install the required packages using pip. (Consider creating a `requirements.txt` file for easier installation).
    ```bash
    pip install pandas numpy tensorflow scikit-learn
    ```

## 6. Usage Instructions
1.  **Prepare the Data:** Ensure your dataset is correctly placed in the `Dataset/` directory or update the paths in the scripts accordingly.
2.  **Run the Detection Script:**
    Execute the main script to perform energy theft detection.
    ```bash
    python ElectricityTheftDetection.py
    ```
    Alternatively, on Windows, you can use the provided batch file:
    ```bash
    run.bat
    ```
3.  **Testing:**
    To test the model with the provided test data, run:
    ```bash
    python test.py
    ```

## 7. Model Details
The model architecture is defined in `model/model.json`, and the trained weights are stored in `model/model_weights.h5`. The model is trained to classify consumption patterns as either 'normal' or 'theft'.

## 8. Contributing
Contributions to improve the project are welcome. Please follow these steps:
1.  Fork the repository.
2.  Create a new branch for your feature or bug fix.
3.  Commit your changes with clear messages.
4.  Submit a pull request.

## 9. License
MIT License
