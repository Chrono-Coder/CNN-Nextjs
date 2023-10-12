# Plan

This project will employ TensorFlow in Python to create a convolutional neural network (CNN) to classify different cat breeds based on their images. The goal is to develop an accurate classifier that can identify a breed from a given image, or perhaps to even give a percentage of different breeds to classify mixed breeds. The final test is to determine the breed of my cat Nala, a mix between a Scottish Fold and a Persian.

The dataset will be downloaded from Kaggle at https://www.kaggle.com/datasets/ma7555/cat-breeds-dataset.

It is an unbalanced dataset of 63 different cat breeds. The images will be preprocessed to be resized to a uniform size, converted to RGB or Grayscale format, and normalized as necessary. Data augmentation techniques like rotation, scaling, and flipping could also be applied to increase the dataset's size and make the model better. Furthermore, the CNN model's hyperparameters could be tuned using techniques such as cross-validation to optimize the loss function and improve its accuracy.
The project aims to build a CNN model using TensorFlow in Python that can accurately classify cat breeds based on their images. The project will involve preprocessing and augmenting the dataset using TensorFlow, building and training a CNN model, and evaluating the model's performance on the validation and testing sets. Finally, with feature extraction from the CNN model I will also train a KNN, SVM, Logistic Regression, and MLP model to compare their performance with the CNN model.

# Results

In the end, due to time constrains I choose a small subset of the dataset to train on my local machine. The subset of data I chose was also unbalanced, which overfitting definitely took place. This could have been several times better if I trained more data and if I had better data.
Overall, I did get an ROC score of 87% so this is still way better than flipping a coin for prediction. Due to the class imbalance however, during testing the accuracy was quite low. I could also just have done transfer learning from an existing model such as the VGG-16, but I really wanted the full experience of doing everything from scratch. The experience has taught me a lot and I understand my mistakes and know where to improve for the future.

For fun I decided to create a simple webpage that uses the model I trained to make predictions on images of cats. The webpage can be found at https://cat-predictor.vercel.app.
