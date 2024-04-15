# Face-recognition-using-OpenCV-
Face recognition using OpenCV involves detecting faces, aligning them, extracting features, and using a recognition model to identify individuals. OpenCV provides tools for each step, enabling the creation of robust face recognition systems with applications in security, surveillance, and biometrics.
# Real-Time Face Detection with OpenCV
Installing OpenCV for Python To install the OpenCV library, simply open your command prompt or terminal window and run the following command pip install opencv-python

Step 1: Pre-Requisites First, let’s go ahead and import the OpenCV library and load the Haar Cascade model just like we did in the previous section.

Step 2: Access the Webcam Now, we need to access our device’s camera to read a live stream of video data. This can be done with the following code Notice that we have passed the parameter 0 to the VideoCapture() function. This tells OpenCV to use the default camera on our device. If you have multiple cameras attached to your device, you can change this parameter value accordingly.

Step 3: Identifying Faces in the Video Stream Now, let’s create a function to detect faces in the video stream and draw a bounding box around them,The detect_bounding_box function takes the video frame as input. In this function, we are using the same codes as we did earlier to convert the frame into grayscale before performing face detection. Then, we are also detecting the face in this image using the same parameter values for scaleFactor, minNeighbors, and minSize. Finally, we draw a green bounding box of thickness 4 around the frame.

Step 4: Creating a Loop for Real-Time Face Detection Now, we need to create an indefinite while loop that will capture the video frame from our webcam and apply the face detection function to it
