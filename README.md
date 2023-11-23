# Stock-Price-Prediction
This comprehensive code snippet describes a project on stock price prediction using Multi-Layer Perceptrons (MLPs) for three different stocks (Apple, Cisco, and GE). The project is structured into several key components:

## Data Setup and Preprocessing:

Stock data for Apple (AAPL), Cisco (CSCO), and GE is read from CSV files and processed.
The data includes dates, times, and closing prices.
Missing values are filled with the mean of the respective columns.
The data is filtered for a specified date and time range.
Pivot tables are created for each stock to organize data by date and time.

## Data Visualization:

Normalized closing prices and intraday prices are plotted to visualize stock performance over time.
A correlation matrix is computed and visualized to understand the relationship between different stocks' closing prices.
Principal Component Analysis (PCA):

PCA is applied to standardize the data (mean 0, standard deviation 1) and reduce dimensionality.
The number of components is chosen to capture 95% of the variance.

## MLP Model Setup and Tuning:

Three separate MLP models are constructed for each stock.
Input features for the MLPs are created using the principal components obtained from PCA.
The models are trained and tuned using TensorFlow.
Hyperparameters such as layer size and batch size are varied to optimize performance.
Training involves computing loss, applying gradient descent, and adjusting weights.

## Model Evaluation:

Each MLP model is evaluated by predicting stock prices and calculating the relative prediction error.
Relative prediction error (REP) is the absolute difference between predicted and actual prices relative to actual prices.
Plots of REP against time are generated to visually assess model performance.

## Summary Tables:

Summary tables are created to consolidate key performance metrics like training and test MSE, runtime, and best epoch across different hyperparameter settings.
Overall Problem and Method:
The project tackles the challenge of predicting stock prices using historical data. It employs a methodical approach starting from data preprocessing, visualization, PCA for feature engineering, followed by designing, training, and tuning MLP models. The approach demonstrates a blend of data analysis, machine learning, and deep learning techniques to address a complex financial prediction problem.

## Results:
Each MLP model's performance is summarized in terms of relative prediction error, providing a quantitative measure of how well the model predicts future stock prices. The plots and summary tables offer insights into the models' accuracy and efficiency, making it easier to compare different configurations and understand each model's strengths and limitations.
