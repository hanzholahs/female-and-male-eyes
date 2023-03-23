# Deep Learning Classifier: Case Study on Images of Female and Male Eyes

by [Hanzholah Shobri](https://github.com/hanzholahs), 20 March 2023

### Project Description

This is a report of the process of building a neural network classifier model that could differentiate between images of male and female eyes. The dataset for the problem can be accessed via [Kaggle](https://www.kaggle.com/datasets/pavelbiz/eyes-rtte). This analysis loosely followed the universal workflow of machine learning, as demonstrated by Chollet (2018).

The dataset contains a total of 11,525 coloured images (which can be represented with the colours red, green and blue) of female and male eyes collected by Pavelbiz (2021). The images have varying resolutions (different pixel numbers for its height and weight dimensions). There are two classes or labels for the dataset: male and female. For this analysis, the images were assumed to be representative of the population of eyes.

To build the model, the analysis leveraged a set of development tools in `TensorFlow` library. The model used different types of layers, mainly the fully connected and convolutional layers. The performance of the model was evaluated from its accuracy in predicting the label of a given picture, and the validity of the hypotheses were evaluated based on this metric. The evaluation protocol being employed for the optimal model selection in this analysis was the hold-out validation set. 

The optimal, final model was fitted to the complete set of the training data and assessed using the test data. The same model with identical architecture and configurations was also trained using augmented data (with randomly transformed images of the training data) and evaluated using the same testing data. The performances of both trained models were then compared.

The final model could achieve more than **92% accuracy**, and using data augmentation could improve the performance for about 5% increase.


### References

Chollet, F., 2018. Deep learning with Python. Manning Publications, Shelter Island.

Pavelbiz, 2021, Female and male eyes. URL: https://www.kaggle.com/datasets/pavelbiz/eyes-rtte (accessed 3.13.23).
