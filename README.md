# DeepFake_FaceRecognition
Machine learning project using python to recognize fake and real faces

The following code works in two parts. In the first part we create the data for each picture (1024x1024) by turning them into grey scale, calculating 2-DFT, center them with fftshift, calculate the magnitude, and at last calculate the radial average for each picture. Once we have each pictures data we can start training (real and fake) our classifier with the training data which will be done with the gradient descent with the learning algorithm. Once our classifier has been trained we may insert test pictures to get their results which will be saved into a file.
