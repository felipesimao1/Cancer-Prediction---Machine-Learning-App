# Breast Cancer Prediction App and Model

This repository contains two main components: the breast cancer prediction app (`app.py`) and the code for training and saving the prediction model (`model.py`). Below are details for each component:

## Breast Cancer Prediction App (`app.py`)

The `app.py` is a web interface built using Streamlit. It allows users to predict breast cancer based on cellular nuclei measurements. Here are some highlights:

### Features

1. **Interactive Sidebar:** Users can adjust the values of cellular features using sliders in the sidebar.

2. **Radar Chart:** Displays an interactive radar chart representing the selected features.

3. **Prediction Output:** Provides a prediction on whether the cell is benign or malignant along with probabilities.

4. **Observation:** This application is for academic purposes. It should never be used for official medical decisions.


### How to Use

1. Clone the repository to your local environment:

   ```bash
    git clone https://github.com/your-username/your-repository.git
    
    pip install -r requirements.txt

    streamlit run app.py

Open your browser and navigate to the link provided by Streamlit (typically http://localhost:8501).

Use the sidebar to adjust cellular feature values and observe the radar chart and prediction.

Note: This app is for educational purposes only. Do not use it to make medical decisions.

# Breast Cancer Prediction Model (model.py)
The model.py file contains code to train and save a breast cancer prediction model. Here is an overview of the training process:

## Training the Model
Loading Data: The dataset is loaded from the data/data.csv file.

Data Preprocessing: Unnecessary columns are dropped, and the target variable (diagnosis) is mapped to binary values (Malignant: 1, Benign: 0).

Scaling Data: The data is standardized using StandardScaler.

Model Training: Logistic Regression is used to train the model.

Saving the Model: The trained model and scaler are saved using Pickle.

Note: Ensure that the necessary Python libraries are installed before running the script.

Project Structure
app.py: Main code for the prediction app.
model.py: Code for training and saving the prediction model.
data/data.csv: Dataset used by the app and model.
model/model.pkl: Trained prediction model.
model/scaler.pkl: Scaler used for data normalization.
[dataset link: ](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)

How to Train the Model
Run the following command:

   ```bash
   python model.py