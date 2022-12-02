# Stock_Prediction_CNN
Building Images out of High Frequency Stock Data to make Return Forecasts using a Convolutional Neural Network

*Important Disclaimer: I know this can be coded MUCH more efficient, back then I was still very early in the learning curve. Maybe I'll improve the code if I find the time in the future. I have learned a lot since starting my data science masters degree.*

This is my first major project in python/ jupyter. I know that there is a lot of stuff that can be improved in my code. I want to use github to document my journey as I transition from a Finance and Economics Bachelor to a Data Science Master Program. So more projects and (hopefully) improved code to come.

The files show different versions of the CNNs on an example stock, as well as the code used for a comparison against an ARIMA model.

CNN1: One-Day Input, no retraining within the forecasting period

CNN2: One-Day Input, retrained for each prediction in the forecasting period

CNN3: Three-Day Inout, no retraining within the forecasting period

I completed this project for my Bachelor Thesis. The abstract reads as follows:

The accurate prediction of stock returns can improve investment performance for practitioners in finance as well as help academics explain the behavior of financial markets. Contributing to the vast research in this area, we are forecasting the daily mean returns of four different stocks. Our raw predictor data consists of nine observations for each minute of the preceding trading day. The data is utilized by transforming it to form two-dimensional images, with the height representing the number of minutes on the given trading day and the width representing the nine observations made each minute. These images are then fed to a convolutional neural network. We propose three different versions of our model. The first one is always receiving one day worth of high frequency data and predicts the whole forecasting set this way. The second model is retrained for each forecast including all available data for that day. Lastly, we provide the model with a three-day input, achieving the best results. The predictive abilities of all three models exceed the results obtained using an autoregressive integrated moving average model. While the mean squared error ranks similar for both methods, the convolutional neural networks produce more accurate forecasts in terms of the direction and in terms of the algebraic sign of the returns.
