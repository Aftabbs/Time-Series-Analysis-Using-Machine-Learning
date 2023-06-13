# Time-Series-Analysis-Using-Machine-Learning
* Time Series Forecasting of Hourly Energy Consumption
![image](https://github.com/Aftabbs/Time-Series-Analysis-Using-Machine-Learning/assets/112916888/ecd9ce56-d4c4-456e-8653-951441266cf7)

This project focuses on performing time series forecasting of hourly energy consumption using machine learning techniques. The dataset used is "PJME_hourly.csv" which contains two columns: "Datetime" and "PJME_MW". The dataset consists of 145,336 rows, capturing the hourly energy consumption readings.

# Project Overview
The main objective of this project is to develop a machine learning model that can accurately forecast the energy consumption based on historical data. By predicting energy consumption, it enables better planning and optimization of resources for energy providers, grid operators, and policymakers. This project provides valuable insights into understanding the patterns and trends in energy consumption, facilitating decision-making and resource allocation in the energy sector.

# Project Steps
* Data Exploration: The project begins with exploring the dataset to gain insights into the energy consumption patterns. The "Energy in MW" is plotted against the "Datetime" to visualize the temporal patterns and identify any seasonality or trends.

![image](https://github.com/Aftabbs/Time-Series-Analysis-Using-Machine-Learning/assets/112916888/75ae6a2f-3cdd-4bd5-ba18-800043ae57af)

* Data Splitting: The dataset is split into two parts: the training set and the test set. The training set consists of data up to the end of 2014, while the test set includes data from 2015 onwards. This division allows us to train the model on historical data and evaluate its performance on unseen future data.

![image](https://github.com/Aftabbs/Time-Series-Analysis-Using-Machine-Learning/assets/112916888/6864e6ca-eb7e-41b2-87f2-d8659ae95fab)

* Feature Creation: In order to capture additional temporal patterns, relevant features are created from the "Datetime" column. Features such as hour, day, week, month, and year are extracted to incorporate seasonality and long-term trends into the model.

* Model Development: XGBoost regressor is chosen as the machine learning algorithm for this project. XGBoost is known for its strong performance in time series forecasting tasks. The model is trained on the training set using the provided features and the corresponding energy consumption values.

* Model Evaluation: The trained model is evaluated using the test set. The root mean squared error (RMSE) is calculated to measure the prediction accuracy of the model. The lower the RMSE value, the better the model's performance.

* Feature Importance: The feature importance of the model is analyzed to identify the most influential features. This analysis helps in understanding which temporal factors have a significant impact on energy consumption. In this project, the "Month" feature is identified as an important factor.

![image](https://github.com/Aftabbs/Time-Series-Analysis-Using-Machine-Learning/assets/112916888/c6c8bd83-7f23-47a6-91d1-2d96907b65cd)

* Visualization: Meaningful visualizations are created to present the findings and insights from the project. Visualizations can include time series plots, feature importance plots, and any other relevant graphs that enhance the understanding of the data and the model's performance.

![image](https://github.com/Aftabbs/Time-Series-Analysis-Using-Machine-Learning/assets/112916888/085ff4a3-10bc-4a34-a7fe-111c7df6d15d)

![image](https://github.com/Aftabbs/Time-Series-Analysis-Using-Machine-Learning/assets/112916888/99559921-e89a-4135-9e2d-9e555193419c)


# Enhancements and Industry Use Case
* Forecasting Accuracy Improvement: The project can be enhanced by exploring and incorporating other advanced time series forecasting techniques such as SARIMA, Prophet, or LSTM models. These models may capture complex patterns and dependencies in the data, potentially improving the forecasting accuracy.

* Demand Planning and Resource Allocation: Accurate energy consumption forecasting is crucial for demand planning and resource allocation in the energy sector. This project provides a foundation for developing a robust forecasting system that can aid energy providers in optimizing their resource allocation strategies, ensuring sufficient supply to meet the demand.

* Load Balancing and Grid Management: Effective energy consumption forecasting helps grid operators in managing the electricity grid more efficiently. By predicting peak demand periods and load patterns, grid operators can optimize load balancing, reduce network congestion, and ensure reliable energy supply.

* Renewable Energy Integration: Time series forecasting of energy consumption is also essential for integrating renewable energy sources into the grid. By accurately predicting energy demand, renewable energy generation can be better planned and coordinated, enabling a smooth transition to a more sustainable energy mix.







