# DeepWay
This project is an aid to the blind. Till date there has been no technological advancement in the way the blind navigate. So I have used deep learning particularly convolutional neural networks so that they can navigate through the streets. 
# My Approach 
## Collecting Training Data
My project is an implementation of CNN's, and we all know that they require a large amount of training data. So the first obstruction in my way was a correclty labeled dataset of images. So I went around my college and recorded a lot of videos(of all types of roads and also offroads).Then I wrote a basic python script to collect save images from the video(I saved 1 image out of every 5, because the consecutive frame are almost identical). I collected almost 10000 such images almost 3300 for each class(i.e. left right and center). 
Left image:



## Training the Model
I made a collection of CNN architectures and trained the model. Then I evaluated the performance of all the models and chose the one with the best accuracy. I got a training accuracy of about 97%
The architecture of the best model was:


##
   ![screenshot 247](https://user-images.githubusercontent.com/24778913/41226545-6982ca30-6d8f-11e8-88d2-b771b3647e54.png)
   ##
   
## Interfacing with the Arduino
The next problem was how can I tell the blind people in which direction to move .
So I connected my python program to an Arduino. I connected the servo motors to arduino and fixed the servo motors to the sides of an spectacle.  Using Serial communication I can tell the arduino which servo motor to move which would then press to one side of the blind person's head and would indicate him in which direction to mode