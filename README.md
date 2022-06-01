# Face-Recognition-Web-App-with-Machine-Learning-in-Flask
It is an Machine Learning Model which detects faces and classifies the gender.

Dataset has been uploaded on this link named Module-2: https://drive.google.com/file/d/1zq9nDKb0LGYRxXLVeh1032pBjhTqNXnH/view?usp=sharing


Relevant HTML Files have been uploaded on this link named Module-4 : https://drive.google.com/file/d/1smo8cZJsprjIw4sNCLf1AQVT3T8g6CE2/view?usp=sharing

This ML Model is integrated with Flask app. As soon as user uploads the image,it identifies its gender.


ML Model application flow:
a) Initially we have highly unstructured data,since images are of different sizes.So first we need to extract the male and female images and crop them using haar cascade classifier and then save them to respective male_crop and femal_crop folders.

