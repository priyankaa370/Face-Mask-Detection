# Face-Mask-Detection
This project determines if a person is wearing a face mask or not using the Machine Learning model - Faster RCNN.

**TRAINING**

For both the training and detection tasks, python programming language and
Google Colaboratory platform is used. A dataset was created to train the model.
The dataset was then divided into 2 parts for training and testing purpose. The
training of the model is done using the training part of the dataset. The flow of
training the dataset is:

• First, training and testing images is saved in two distinct folders
• Then train.csv and test.csv files are generated.
• These .csv files are then converted to TF record files since Tensorflow is used.
• Import dependencies such as tf-models-official, tf-lim, tensorflow.io, lvis etc.
• Save the configuration file from the Tensorflow Detection Model Zoo, where pretrained models are available.
• Then train the model using the dataset while continuously reducing the learning rate.

**DETECTION**

In this section, the main task of the model which Object Detection which is
implemented using Faster R-CNN is discussed. This process is done in a step by
step manner and the programming is done using Python Language. Instead of
showing the entire code directly, an explanation is provided to let the reader
understand in more better and interesting way. The Flow of the Detection is such
that:

• For the images, save the test image in a destination folder or capture the video through webcam
• Import all the required dependencies mathlib, pycocotools etc
• Compile protobuf to configure model and training parameters and install object detection module
• Capture each frame from this video and pass it through the saved model
• Get the boxes and the scores. Draw coloured rectangles around the detected objects.

As the backbone for the base model, ResNet50 architecture is used for the training of the Faster R-CNN model. The pretrained model was taken from the Tensorflow Object Detection Model Zoo and the training steps are kept as 10,000. The dataset used for training the model contains 853 images with different situations belonging to 2 classes i.e. with mask and without mask.
