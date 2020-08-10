# FaceRecognition-Using-OpenCV
Face Recognition using OpenCV in Python

In order to build our OpenCV face recognition pipeline, we need to apply deep learning in the following key steps:

 - To apply **face detection**, which detects the presence and location of a face in an image, but does not identify it.
 - To **extract faces** from the images.
 - Train the model with the images and **classify them**.
 - Test the model with **test images**.
 
# The Dataset

Here,The dataset used contains images of two people:

  - Zayn Malik.
  - Gigi Hadid.
  
The images folder contains two folders:

  - 0 (Images of Zayn collected from internet)
  - 1 (Images of Gigi collected from internet)
  
# The Face Recognizer Used

Local Binary Patterns Histograms (LBPH) – **cv2.face.createLBPHFaceRecognizer()**

The idea with LBPH is not to look at the image as a whole, but instead, try to find its local structure by comparing each pixel to the neighboring pixels. 

# Recognition Process

Later during recognition, the process is as follows:

  - Feed a new image to the recognizer for face recognition.
  - The recognizer generates a histogram for that new picture.
  - It then compares that histogram with the histograms it already has.
  - Finally, it finds the best match and returns the person tag associated with that best match.
  
