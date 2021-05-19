# face-mask-detector

This project aims to recognize people who are wearing a mask or not, the distinctive colors for recognition are green for the person who uses a mask and red for those who do not.

The project is divided into the following parts:

Dataset: contains 2 folders with images in JPG format of sample of people wearing masks and people without using them. All these images will be processed and used to train the model that will perform the subsequent recognition.

Face detector: Files used for the face-detection algorithm in the detect_mask_video file

train_mask_detector.py: Python file that will train the model using the images that we have added in the dataset section

detect_mask_video.py: Python file in charge of performing the recognition on an already trained model from the sample images.

mask_detector.model: Python model on which we will work

requirements.txt: Installation requirements file for the correct compatibility of the project

plot.png: Sample plot and its level of loss and precision

cropped_faces: Directory that will contain the images of people who do not wear a mask (it will be created automatically after running "facedetector.py")

face-detector-demo: Demo in mp4 format

Installation and requirements:

Anaconda Pycharm Internet connection Intermediate python knowledge Webcam

Installation process:

First of all we need to satisfy the requirements on the "requirements.txt" file, we can install them by running "pip install -r requirements.txt" with the anaconda interpreter.

Then we have to execute the train class which will train the model train_mask_detector.py. The training process will take about 20 minutes.

Once the model has finished its training we have to execute the python file detect_mask_video.py.

Now the webcam will be activated and we can use it. If the system detects that you are not wearing your mask it will take a picture of your face and store it on the "cropped_faces" folder.
