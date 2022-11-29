In this project, assume that a local housing society has begun to capture images at the entrance/exit gates and public areas within and around the residential building to recognize the people wearing
a mask from the specific group of people who refuse to comply. 

The data source of this project is the collection of about 12k images, nearly 328.92MB in size. All the photos with the face mask (6K) were scraped from Google, and all the images without the face mask were pre-processed using Jessica Li's Celebrity Face dataset (https://www.kaggle.com/jessicali9530). 

The goal of this project is to classify images and developing a Deep Learning model to recognize if people is wearing face masks or not. 

First, it is important to understander the data. The data set is consist of three folders: Train, Test and Validation. In each folder, the images are further separated by with mask or without mask.

The total number of images in Training set with mask is 5000.
The total number of images in Training set without mask is 5000.
The total number of images in Testing set with mask is 509.
The total number of images in Testing set with mask is 509.
The total number of images in Validation set with mask is 400.
The total number of images in Validation set with mask is 400.


Then, preprocessing the data by rescale the images into a fixed size before inputting to the model, normalizing the value to range from 0-1 by dividing each image by 255. This will let the model train faster and easier when the image is in smaller size.

After preprocessing, build the model to detect the face images are mask or unmask. As this project is image recognition, CNN model is suitable for this. I tried to ResNet50, customized CNN and GoogleNet to compare the result.

Then, compile, train and test the model. 


