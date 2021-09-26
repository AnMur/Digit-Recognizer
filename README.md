# Digit Recognizer

  MNIST ("Modified National Institute of Standards and Technology") is the de facto “hello world” dataset of computer vision. Since its release in 1999, this classic dataset of handwritten images has served as the basis for benchmarking classification algorithms. As new machine learning techniques emerge, MNIST remains a reliable resource for researchers and learners alike. 

 In this repository, I will participate in the 'Digit Recognizer' Kaggle's competition to predict numbers/digits. The data comes from train and test csv files. All digits stored as arrays. To fit them to the convolutional neural network,  I'm going to do some preprocessing: convert digits to np.array as float32, reshape and scale.
 
 I'm going to use convolutional neural network as a main model with 3 convolutional and 2 Dense layers. My model is not going to be very deep only 32 and 64 neurons. My last Dense layer will only have 10 neurons because I have 10 numbers to predict from 0 to 10. My activation functions would be 'relu' except the last 'softmax' for multiclass. My optimizer would be 'adam' with learning rate 0.001. 
 
 The main convern with neural networks is to avoid overfitting. I'm going to use 'Dropout' function and 'MaxPooling'.
 
 After traing my model on train csv, I'm going to predict digits on a new for the model test.csv dataset.
 
### After multiple experimentations with different parameters and number of epochs, my best choise was to stop at the epoch 72 that gives me 0.9933 accuracy score and 0.023 loss.




[Kaggle's Digit Recognizer](https://www.kaggle.com/c/digit-recognizer)


