# Dog Classification Project
This essence of this project is to take an image and say which of 130 different dog breeds is depicted in the picture.  The app includes a check to determine if a human face is detected and if it is, then says what that human looks like.  Dan Aykroyd looks like a Pointer for example.

![DanAykroyd](/DanAckroydDog.png)

This project is part of the [DeepLearning Nanodegree at Udacity](https://www.udacity.com/course/deep-learning-nanodegree--nd101)  

In this project, the baseline of predictions is less than 1%.  This would be the result of random guessing.
The first part of the project is to build a convolutional neural network from scratch.  The architecture is not prescribed so much trial and error is needed.  The end result combines 6 layers of convolutional layers, maxpooling, drop out, batch normalisation, and application of the relu function.  This generates an accuracy of 17%, where the passmark was 10%, both of which are significantly over the baseline rate.

This result was achieved with 12 epochs which took around 20 minutes to run on the GPU machines provided to us by AWS.  

The second element of the project was to better an accuracy of 60% by leveraging pre trained models, ie using Transfer Learning.  Here I took the basis as the VGG16 model which had been trained on the 1000 images on ImageNet, and adjusted the last elements of the model to only predict on the 130 dog breeds.  This generated an accuracy of over 82%, significantly over the 60% criteria.

The final elements of the project required building the algorithm into an app which took in an image file, and then where a human had been detected, identified which dog breed this human resembled, but where a dog was detected, identified which its breed and printed the image and the results out.



