# Anomaly-Detection-Using-LSTM-autoencoder

Authors: [Sayan Hazra](https://github.com/sayan0506) & [Sankalpa Chowdhury](https://github.com/sankalpachowdhury)
LSTM autoencoder based anomaly detection using Keras and Tensorflow backend

* Here in this project we have done a comparative study between **Simple LSTM Network** and **LSTM based Autoencoder Network**. We have tried to detect Anomalies in closing price in **Daily closing prices for S&P 500 index from 1986---&gt;2018**

**Dataset link:** [S&P500 Daily Prices 1986 - 2018](https://www.kaggle.com/pdquant/sp500-daily-19862018)

* The working and intuition behind the LSTM and LSTM Autoencoder can be found from the reference link and Deep Learning Specialization(Sequence Models) course.

* The intuition here is to PASS the time-series window, which predicts the forecasted output for Simple LSTM and Reconstructs the input sequence for LSTM Autoencoder by using Encoder-Decoder network. The main difference is the Latent Space layer or bottleneck layer that exists between encoder and decoder, which helps to reduce dimensionality and better reconstruction approach by low dimensional manifold learning approach.

* The networks are trained similarly, and from the Mean Absolute Error distribution of the predictions on the training set, we set 0.65 as the Threshold error.

* The networks are then used to predict or forecast using original data rather than the normalized one, if the MAE becomes greater than the Threshold, we can detect anomaly correspond to that Date, or the closing proce corresponding to that date holds the Anomaly.

* Details implementation can be found from thr google collab [notebook](https://github.com/sayan0506/Anomaly-Detection-Using-LSTM-autoencoder/blob/main/Anomaly_Detection_Time_Series_Keras.ipynb).

# Reference:

* [LSTM Autoencoder for Anomaly Detection](https://towardsdatascience.com/lstm-autoencoder-for-anomaly-detection-e1f4f2ee7ccf)
* [Step-by-step understanding LSTM Autoencoder layers](https://towardsdatascience.com/step-by-step-understanding-lstm-autoencoder-layers-ffab055b6352)
* [Detecting Mobile Traffic Anomalies Through Physical Control Channel Fingerprinting: A Deep Semi-Supervised Approach](https://www.semanticscholar.org/paper/Detecting-Mobile-Traffic-Anomalies-Through-Physical-Trinh-Zeydan/1b52c7b583cf373008de0cbec1041510d9fe91d2)
* [LSTM Autoencoder for anomaly detection](https://www.youtube.com/watch?v=6S2v7G-OupA)
* [Python Graph Object Module Reference](https://plotly.com/python/creating-and-updating-figures/)
**All the contents are made public, and all modifications, pull requests are welcome but please open issue and discuss before executing any major change in the repository.**
