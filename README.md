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

OUTPUT:
![WhatsApp Image 2022-06-02 at 2 11 09 PM](https://user-images.githubusercontent.com/87833566/171591309-992d2747-f1e4-4a30-bd1f-d89612c1cd58.jpeg)



Once our machine learning model is ready, will we learn and develop a web server gateway interphase in flask by rendering HTML CSS and bootstrap in the frontend and in the backend written in Python.  Finally, we will create the project on the Face Recognition project by integrating the machine learning model to Flask App.

Flask WebPage looks like:

Home Page: <img width="960" alt="image" src="https://user-images.githubusercontent.com/87833566/171593965-e3ec9db4-857b-4bb4-9057-e61f920888a1.png">


FaceApp Page: <img width="959" alt="image" src="https://user-images.githubusercontent.com/87833566/171596970-7f22a647-6879-4390-a947-fc7f4a9c005c.png">


Click on "Try it now!" button and it will redirect to Gender Classification page to Upload and Predict. Then choose the Image file you want to predict and click on "Upload and Predict" button :![WhatsApp Image 2022-06-02 at 2 50 17 PM](https://user-images.githubusercontent.com/87833566/171598863-a5b98543-0fc3-48a2-a82d-dbce7f652ccd.jpeg)






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

