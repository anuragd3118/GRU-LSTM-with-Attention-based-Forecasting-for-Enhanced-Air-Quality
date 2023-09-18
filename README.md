# GRU-LSTM-with-Attention-based-Forecasting-for-Enhanced-Air-Quality
Group Project for Predicting Air Quality Index using Cutting Edge Deep Learning Algorithms for State-of-art results

## Tools and Libraries
- Tools :
#####         Python
#####         Jupyter
- Libraries :
#####        Pandas (1.5.3) — For handling structured data
#####        NumPy (1.23.5) — For linear algebra and mathematics
#####        Scikit Learn (1.2.2) — For machine learning

## Our Machine Learning Model Development Cycle

<p align="center">
  <img width="600" src="" alt="Proposed Attention GRU-LSTM Model ">
</p>

## DataSet
- In this, We have used the Air Quality dataset. This is a dataset that reports on the weather and the level of pollution each hour for five years at the US embassy in Beijing, China. The data includes the date-time, the pollution called PM2.5 concentration, and the weather information including dew point, temperature, pressure, wind direction, wind speed and the cumulative number of hours of snow and rain.

## Steps followed
- Data preparation
- Data Visualization and Normalisation
- Importing the Model
- Fit model along with regularization term
- Evaluate model using various Evaluation Metrics

### Data preparation
- Replace NA values
- Parse date-time into pandas dataframe index
- Specified clear names for each columns

### Data visualization and Normalisation
- Used matplotlib
- Feature Scaling using Min-Max Scaling
- Correlation matrix

### Model preparation
- Normalized data 
- Transformed dataset into supervised learning problem
- Define 2 layer GRU and 2 layer LSTM architecture
- Defined 64 neuron first GRU layer followed by 32 in GRU, 32 in LSTM and last 16 nueron in LSTM
- Add dropout at 20% after every layer
- Added an Attention Layer to focus on datapoints which will then maximise the accuracy

### Model Fitting
- Split data into train and test
- Fitting is done on epochs = 40 and batch_size = 32

### Evaluate model
- Make prediction
- Plot the line graph between actual vs predicted values using plotly (5.15.0)
- Calculate RMSE, MAE, R2 and MSE values

### Results
<div style="float:left">
<div style="float:left"><img src="https://github.com/jyoti0225/Air-Pollution-Forecasting/blob/master/output_graph.png" />
</div>
<br />
