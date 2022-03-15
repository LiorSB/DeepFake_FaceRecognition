# DeepFake_FaceRecognition
Machine learning project using python to recognize fake and real faces

The following code works in two parts.
In the first part we create the data for each picture (1024x1024) by turning them into grey scale, calculating 2-DFT, center them with fftshift, calculate the magnitude, and at last calculate the radial average for each picture.

![image](https://user-images.githubusercontent.com/92099051/158348501-c4344b81-aa4a-4814-8745-d401b4a6dc7e.png)
![image](https://user-images.githubusercontent.com/92099051/158348647-99dfd882-524a-4d3d-bb39-2de6c1638c0b.png)
![image](https://user-images.githubusercontent.com/92099051/158348679-5b202cfb-781c-4178-a688-27a848ec875b.png)
![image](https://user-images.githubusercontent.com/92099051/158348717-6393f7f1-dab4-425d-884a-5789922d6197.png)

Once we have each pictures data we can start training (real and fake) our classifier with the training data which will be done with the gradient descent with the learning algorithm. 

![image](https://user-images.githubusercontent.com/92099051/158348881-400e6b80-4331-4e86-aad6-c81b3d39f859.png)
![image](https://user-images.githubusercontent.com/92099051/158349157-59eedeaa-ead3-4fef-b482-2330bfb749f3.png)

Once our classifier has been trained we may insert test pictures to get their results which will be saved into a file.

![image](https://user-images.githubusercontent.com/92099051/158349205-174cb41e-160e-4c44-8256-0286387e4a4f.png)
![image](https://user-images.githubusercontent.com/92099051/158349272-ef7613c7-ce0e-4fbd-b692-7ede1e784b56.png)
![image](https://user-images.githubusercontent.com/92099051/158349307-b144d5fb-8f02-4489-9b45-d59f2e0e0d50.png)
![image](https://user-images.githubusercontent.com/92099051/158349325-b6f9bc42-5a57-4c6b-bf11-969288ca7068.png)

4 test pictures that were recognized correctly:

![image](https://user-images.githubusercontent.com/92099051/158349584-9d140cef-4619-4fb6-afd5-49bcda7d0042.png)
![image](https://user-images.githubusercontent.com/92099051/158349476-dcfb2f81-5246-422e-9f90-31f3da25c5fb.png)
