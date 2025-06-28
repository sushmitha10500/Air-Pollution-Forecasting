# Air pollution forecasting using lstm on multivariate time series data
Predict PM2.5 pollution levels using historical environmental data with LSTM networks.

------------------------------------------------------------------------------------------------
Built a multivariate LSTM model in Python to forecast air pollution using time series data. Preprocessed data with lag features, normalized inputs, and reshaped for supervised learning. Trained on multiple timesteps, evaluated with RMSE & MAE, and delivered a scalable forecasting pipeline.

Built a deep learning model using Long Short-Term Memory (LSTM) to forecast PM2.5 levels one hour in advance.

Worked with multivariate time series data including temperature, dew point, pressure, wind speed/direction, rain, and snow.

Captured temporal dependencies and trained model using supervised learning techniques.

Demonstrated the effectiveness of deep learning for environmental monitoring and pollution forecasting.

----------------------------------------------------------------------------------------------------------
This project uses the Beijing PM2.5 Data Set, which contains hourly records of air pollution and weather conditions collected over five years at the US Embassy in Beijing, China.
The features include:
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
