# Solar Radiation Prediction

This project uses a hybrid machine learning model to predict solar radiation. The entire workflow, from data preprocessing to model training and evaluation, is contained within a Jupyter Notebook. The trained models and data transformers are saved for potential future use.

***

## 📜 Files in this Repository

* **`Radiation_Prediction_Hybrid.ipynb`**: The main Jupyter Notebook containing all the code for data analysis, preprocessing, model training, and evaluation.
* **`SolarPrediction.csv`**: The dataset used for training and testing the model.
* **`best_radiation_model.pkl`**: A serialized file containing the trained machine learning model with the best performance.
* **`hybrid_model_weights.pkl`**: A file containing the saved weights for the hybrid model component.
* **`imputer.pkl`**: The saved imputer object used to handle missing values in the dataset.
* **`scaler.pkl`**: The saved scaler object used to normalize or standardize the features of the dataset.

***

## ⚙️ Methodology

The project follows a standard machine learning pipeline:
1.  **Data Loading**: The `SolarPrediction.csv` dataset is loaded into the environment.
2.  **Preprocessing**:
    * Missing data points are handled using a saved **imputer**.
    * Numerical features are scaled to a common range using a saved **scaler**.
3.  **Modeling**: A hybrid model is trained on the preprocessed data to learn the patterns and predict solar radiation.
4.  **Evaluation**: The model's performance is evaluated using appropriate metrics, and the best model is saved.

***

## 🚀 Usage

To get started with this project, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/rkb3004/radiation-prediction.git](https://github.com/rkb3004/radiation-prediction.git)
    cd radiation-prediction
    ```
2.  **Install dependencies:**
    You will need a Python environment with Jupyter Notebook. The core libraries can be installed via pip.
    ```bash
    pip install numpy pandas scikit-learn notebook
    ```
    *Note: You may also need a deep learning library like TensorFlow or PyTorch depending on the hybrid model's architecture. Please check the import statements in the `.ipynb` file for a complete list.*
3.  **Run the Jupyter Notebook:**
    Launch Jupyter Notebook from your terminal.
    ```bash
    jupyter notebook
    ```
    Open the `Radiation_Prediction_Hybrid.ipynb` file and run the cells to see the entire process, from data loading to prediction.
