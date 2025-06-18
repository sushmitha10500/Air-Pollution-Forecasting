# Air-Pollution-Forecasting

Built a multivariate LSTM model in Python to forecast air pollution using time series data. Preprocessed data with lag features, normalized inputs, and reshaped for supervised learning. Trained on multiple timesteps, evaluated with RMSE & MAE, and delivered a scalable forecasting pipeline.


This is a dataset that reports on the weather and the level of pollution each hour for five years at the US embassy in Beijing, China.
The data includes the date-time, the pollution called PM2.5 concentration, and the weather information including dew point, temperature, pressure, wind direction, wind speed and the cumulative number of hours of snow and rain.

The dataset contains hourly records collected over five years at the US Embassy in Beijing. The features include:
| Feature | Description                                         |
| ------- | --------------------------------------------------- |
| `No`    | Row index (can be dropped)                          |
| `year`  | Year of the record                                  |
| `month` | Month of the record                                 |
| `day`   | Day of the record                                   |
| `hour`  | Hour of the record                                  |
| `pm2.5` | **PM2.5 pollution concentration** (target variable) |
| `DEWP`  | Dew Point                                           |
| `TEMP`  | Temperature                                         |
| `PRES`  | Atmospheric Pressure                                |
| `cbwd`  | Combined Wind Direction                             |
| `Iws`   | Cumulated Wind Speed                                |
| `Is`    | Cumulated Snow hours                                |
| `Ir`    | Cumulated Rain hours                                |

Using this data and framed a forecasting problem where, given the weather conditions and pollution for prior hours, we forecast the pollution at the next hour.
