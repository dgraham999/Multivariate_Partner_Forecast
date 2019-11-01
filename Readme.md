These programs require:
Latest distribution of Anaconda Python 3 with sklearn.
After updating Anaconda additionally update Tensorflow and Keras.  Anaconda lags the latest versions.
Install 'holidays' with pip.  Not in Anaconda.
Install sklearn-pandas with pip for the DataFrameMapper function.  DataFrameMapper is imported from the module sklearn_pandas.

This code combines both continuous and categorical variables in a dense neural network coded in TensorFlow/Keras using the functional api.
There is no data so the code must be modified for your purposes.
The prediction has two examples:  the target variable is scaled using minmax or the by the log.
In this particular example the target log yields a 3% mape on the validation set.  The minmax scaler yields a 13% mape error on the validation set.  Both should be tried when introducing new data.
