# Dataset
The dataset is provided by WideBot as a Classification Task
# Approaching-Dataset
- Checked for the missing values and deleted it, because ML doesn't do well with missing data
- There are features that consists of characters, it needed to be encoded into numerical classes for further manipulation and feeding it to    the model in the future
- I checked the correlation between each pair of features to get an insight about the data, and compared it to the Y label to see which        contributes more to it
- There's a fully correlation in the training set between variable19 and classLabel so the algorithm can learn to predict according to   variable19 value and get a 100% accuracy on the dataset, which this might not be the case in general, and dropping this feature drops the CV accuracy dramatically
- I tried a few Models SVM, RandomForests and LogisticRegression, but the one that showed best accuracy on the training and validation set   was LogisticRegression
- The training set accuracy = 0.92 and validation set = 0.72, this means the data is overfitting
- after trying to manipulate the features to avoid overfitting the accuracy only got worse
- Though validation set accuracy is acceptable, we need more data to be able to minimize or avoid the overfitting.
# NOTE: 
check link below if the notebook is not working on github
https://nbviewer.jupyter.org/github/omarbassuni2/Binary-Classification-Problem/blob/master/Binary%20Classification.ipynb
