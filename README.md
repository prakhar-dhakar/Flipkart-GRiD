# Flipkart-GRiD

Problem Statement
The 2019 GRiD challenge for students is to leverage a pre-defined data-set from Flipkart to enable ‘Vertical Classification’ using images.

Flipkart Object Localization Challenge

Flipkart Object Localization Challenge consists of developing a model that localizes (identifies the bounding box) the object in an image. Simply put, given an image, the model should produce coordinates of the rectangle where in the object lies (refer Figure 1).  

![alt text](https://s3.ap-south-1.amazonaws.com/d2c-cdn-mumbai/uploads/images/image1.jpg)

Figure 1. Localizing the Object in the Image

You will be provided a data set which has images and a metadata file containing the name of the image and bounding box (x1, x2, y1, y2) around the object in the image.  Your model should take as input an image and produce the coordinates of the bound box.

Your model will be validated against a blind set, which will be shared with you which will contain only the images.

The performance metric used is mean intersection over union of the areas (amongst the rectangle you produce vs. the ground truth), refer Figure 2.

![alt text](https://s3.ap-south-1.amazonaws.com/d2c-cdn-mumbai/uploads/images/image2.jpg)

Figure 2. Intersection over Union = 4/14

 

Data Description

You’re given two different files - Training.csv and Test.csv. The training data set consists samples to train your model. The test data set should be used for submission after predicting bounding box dimensions and same will be used for evaluations. You can download the image data set for the set of all the images you'll require during the challenge. 

Please note that the image data set is a huge file of around 13 GB.

Variable	Description
image_name	image name
x1	x position of the bounding box
x2	x+width of bounding box
y1	y position of the bounding box
y2	y+height of bounding box
 

Submission File Format

Participant needs to submit the predication file (test.csv) containing the Image Name and the corresponding bounding box values associated with that image in the .csv format
