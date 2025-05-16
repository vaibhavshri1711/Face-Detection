# Face-Detection

This face detection project uses Python and OpenCV to identify human faces in images. The core of the project is based on the Haar Cascade Classifier, a pre-trained model provided by OpenCV for object detection. Haar cascades are effective for detecting frontal faces using a feature-based approach.

The process begins by loading an image using cv2.imread(), followed by converting it to grayscale, as Haar cascades work best on single-channel images. The Haar cascade XML file for frontal face detection is then downloaded and loaded into the program using cv2.CascadeClassifier().

Once the image and classifier are ready, the program uses the detectMultiScale() method to locate faces in the image, returning coordinates and sizes of any detected faces. These coordinates are used to draw bounding boxes (rectangles) around each detected face using cv2.rectangle().

Finally, the annotated image is displayed using cv2_imshow() (especially useful in Google Colab), showing red boxes around each face found. This simple yet powerful project demonstrates how pre-trained models can be used for real-time applications like face detection with minimal code.
