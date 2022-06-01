# Face-Recognition-Web-App-with-Machine-Learning-in-Flask
It is an Machine Learning Model which detects faces and classifies the gender.

Dataset has been uploaded on this link named Module-2: https://drive.google.com/file/d/1zq9nDKb0LGYRxXLVeh1032pBjhTqNXnH/view?usp=sharing


Relevant HTML Files have been uploaded on this link named Module-4 : https://drive.google.com/file/d/1smo8cZJsprjIw4sNCLf1AQVT3T8g6CE2/view?usp=sharing

This ML Model is integrated with Flask app. As soon as user uploads the image,it identifies its gender.


ML Model application flow:

a) Initially we have highly unstructured data,since images are of different sizes.So first we need to extract the male and female images and crop them using haar cascade classifier and then save them to respective male_crop and femal_crop folders.

b)Now the cropped images are highly unstructured,so we have to resize them so that we can train the model easily. From EDA,we get the min size as 54,so we remove the images less than size 54 and resize rest to 100x100.
While Resizing ,I first read the image,then converted it into gray scale ,then resized it into 100x100 array and then flattened (1x10,000) it.

c) After the data is structured, lets pre-process the data using MinMax Scaling:

Xnorm= (X-minvalue)/(maxvalue-minvalue)

So data is normalised now.


d) For the preprocess images, we will extract features from the images, ie. computing Eigen images using principal component analysis. With Eigen images, we will train the Machine learning model and also learn to test our model before deploying, to get the best results from the model we will tune with the Grid search method for the best hyperparameters.



Once our machine learning model is ready, will we learn and develop a web server gateway interphase in flask by rendering HTML CSS and bootstrap in the frontend and in the backend written in Python.  Finally, we will create the project on the Face Recognition project by integrating the machine learning model to Flask App.

Summary:
Following things have been used in this project:
-Python

-Image Processing with OpenCV

-Image Data Preprocessing

-Image Data Analysis

-Eigenfaces with PCA

-Face Recognition Classification Model with Support Vector Machines

-Pipeline Model

-Flask (Jinja Template, HTML, CSS, HTTP Methods)

-Finally, Face recognition Web App

