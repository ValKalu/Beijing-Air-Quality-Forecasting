# Beijing-Air-Quality-Forecasting

Beijing Air Quality Forecasting Project Overview
This project is a graded assignment for the Machine Learning Techniques I course, focusing on the critical task of forecasting PM2.5 (fine particulate matter) air pollution levels in Beijing. We utilize the power of Recurrent Neural Networks (RNNs) and Long Short-Term Memory (LSTM) models, which are particularly well-suited for time-series data analysis.

Accurate prediction of PM2.5 concentrations is paramount for effective environmental policy-making, safeguarding public health, and enabling timely interventions such as issuing health advisories or implementing traffic regulations.

# Project Objectives
The core objectives pursued in this project include:

Data Preparation

Model Development

Performance Optimization

Evaluation

Prediction Generation

# Project Description Best Performing Model
Through a series of experiments and iterative refinements, the following LSTM-based model architecture demonstrated the most promising performance in minimizing RMSE and ensuring good generalization on unseen data.

# LSTM Architecture
First LSTM Layer:

Units: 128

Activation: [ReLU]

Regularization: [L2]

Dropout Layer: [20% (0.2)]

Second LSTM Layer:

Units: 64

Activation: [ReLU]

Regularization: [L2]

Dropout Layer: [20%]

Dense Layer:

Units: [32]

Activation: [ReLU]

Regularization: [L2]

Output Layer:

Units: 1 (for PM2.5 prediction)

Activation: linear (for regression)

# Data Preparation Training Configuration
Optimizer: [Adam]

Learning Rate: [0.001]

Loss Function: Mean Squared Error (MSE)

Evaluation Metric: Root Mean Squared Error (RMSE): 70.65

Training Epochs: [10]

Batch Size: [32]

Validation Split: [0.2]

# Repository Structure
.

├── data/     
├── models_output/                    
├── notebook/                               
├── README.md                   
└── submission.csv              

# Setup Instructions
To get this project up and running on your local machine or in a Google Colab environment, follow these simple steps:

1. Clone the Repository:

git clone [(https://github.com/ValKalu/Beijing-Air-Quality-Forecasting)]
cd [Beijing-Air-Quality-Forecasting]

Replace [(https://github.com/ValKalu/Beijing-Air-Quality-Forecasting)] and [Beijing-Air-Quality-Forecasting] with your actual GitHub repository details.

2. Download Data:

Obtain the train.csv, test.csv, and submission.csv files directly from the Kaggle competition page. Place these files into the data/ directory within your cloned repository.

3. Install Dependencies:

Ensure you have Python 3 installed. You can install the necessary Python libraries by running:


!pip install pandas numpy matplotlib tensorflow scikit-learn


4. Run the Jupyter Notebook:
Navigate to the notebook/ directory (or wherever your main notebook is located) and open Air_Quality_Forecasting_in_Beijing_1.ipynb in a Jupyter environment (Jupyter Lab or Jupyter Notebook). Execute all cells sequentially. If running in Google Colab, ensure you mount your Google Drive to access the datasets as specified in the notebook.

# Contributor
# Valentine Kalu

