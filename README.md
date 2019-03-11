
# Predicting Flower Picture with AutoML

### [Colab Link](https://colab.research.google.com/drive/1y5weLPsAJ5cIElYPy4qMQ9athQgSbLvz)

### Objective
In this notebook, I aim to use Google AutoML Vision to train classification model for picture labeling. I firstly trained the model with 3667 labeled pictures. The evaluation has a precision rate of 95.687%. Further, I tested the model with three pictures randomly found on the Internet, and AutoML got all of them!

### Modeling
1. Vision ImageAnnotator API
The comprehend API returns the most likely sentiment for the text as well as the 
The ImageAnnotator has built-in model, hence do not require user to train one’s own model in order to label the picture. With the input of a picture of daisy, the output is as follows, which is quite precise.
![alt text](https://github.com/elaine-chenma/AutoML/blob/master/pics/Picture0.png)

2.  AutoML Vision trained model
I used three randomly chosen pictures to test the classification accuracy of the trained model. The model returns the correct label with 99.9% confidence, which is quite amazing.
![alt text](https://github.com/elaine-chenma/AutoML/blob/master/pics/Picture1.png)
![alt text](https://github.com/elaine-chenma/AutoML/blob/master/pics/Picture2.png)

### Recommendation for Cloud User
If we have a bunch of unlabelled pictures and want to have them labelled and have a general understanding of what’s in the pictures, Vision ImageAnnotator is a plug-in tool.
If we have labelled training data and want to perform a classification task based on existing knowledge, AutoML Vision allow users to build their own model and predict new items.
