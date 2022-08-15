# epsil
Application of Machine Learning in Finance Domain like Stocks/Assets trend prediction, Anomaly detection, Volatility Estimate.

### Finance Algorithms:
1. [Stock Trend Prediction](https://github.com/HSaurabh0919/epsil/blob/main/Finance/TrendPrediction_01.ipynb) as a Classification Problem with DecisionTreeClassifier and GradientBoostingClassifier.
2. [Forex Trading](https://github.com/HSaurabh0919/epsil/blob/main/Finance/forex_trading.ipynb) using LSTM, GRU and CNN.
3. [Asset Allocation](https://github.com/HSaurabh0919/epsil/blob/main/Finance/asset_allocation.ipynb) using One Step Prediction from Random Forest and Linear Regressor and using Buy and Hold Strategy as a baseline.


### Forex Trading Results (Regression Formulation)
#### Default Values:
| Feature | Value|
| ----------- | ----------- |
| Sequence length | 60       |
| Number of Layers | 4      |
| Droput Value | 0.2       |
| Sequence length | 60       |

#### Performance
| Architecture | R-squared Score|
| ----------- | ----------- |
| Stacked GRU      | 0.40       |
| Stacked LSTM     | -1.29       |
| Stacked CNN     | -0.02       |
| Stacked CNN with 10 layers     | 0.23       |
| Stacked GRU with Added Features   | -0.31        |
| Stacked GRU + LSTM with Added Features   | -15.6        |

### Forex Trading Results (Classification Formulation)
#### Default Values:
| Feature | Value|
| ----------- | ----------- |
| Sequence length | 60       |
| Number of Layers | 4      |
| Droput Value | 0.2       |
| Sequence length | 60       |


#### Performance
| Architecture | Accuracy Score|
| ----------- | ----------- |
| Stacked GRU  with single feature   | 0.60       |
| Stacked GRU with Partial Added Features   | 0.58        |
| Stacked GRU + LSTM with 10 Added Features   | 0.51        |
| Stacked GRU  with single feature and sequence length 4  | 0.51       |

### Asset Allocation Results
| Strategy | Annual Returns | Accuracy Volatility | 
| ----------- | ----------- | ----------- |
| Buy and Hold Strategy  | 17.25%       | 15.96% |
| Asset Allocation using LR Predictions | 21.93% | 14.82% |
| Asset Allocation using LR Predictions  | 17.69% | 13.75% |


### Anomaly Detection
1. [Anomaly Detection](https://github.com/HSaurabh0919/epsil/blob/main/Anomaly_Detection/autoencoder.ipynb) using Autoencoders on a private datatset.
2. [Anomaly Detection](https://github.com/HSaurabh0919/epsil/blob/main/Finance/Anomaly_Detection/Anomaly_detection_01.ipynb) using Isolation Forest(Unsupervised Learning) on a simple dummy dataset
