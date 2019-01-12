# tensorflow_churn
The Jupyter notebook contains code to predict whether telco customers churn or not. Since customers either cease or continue their relationship with the telco company, the classification problem is a binary one. Features used to predict churn include customer account information (e.g. monthly charges) and demographic information (e.g. gender).

The Jupyter notebook is split into three parts.

In part 1, I explore, visualize, and preprocess the data. I also engineer 3 new features using principal components analysis.

In part 2, I build a neural network using TensorFlow, train the network, and use it to generate predictions on the test dataset. The model managed to achieve a test accuracy of 80.0%, which is higher than the benchmark accuracy of 73.4% (in the dataset, 73.4% of customers did not churn).

In part 3, I fit 7 different models (random forest, xgboost, adaboost, light GBM, K-nearest neighbors, support vector machine, and logistic regression) to the training data, then use a hard voting classifier to stack these models together. Random forest produced the worst performance (76.3% accuracy) on the test set, whereas logistic regression produced the best performance (81.2% accuracy). The stacked model achieved a test accuracy of 80.0%.

The data can be accessed from: https://www.kaggle.com/blastchar/telco-customer-churn/home
