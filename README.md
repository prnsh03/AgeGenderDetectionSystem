# Age Gender Detection System
## Age and Gender Detection System

### Overview

This project implements an age and gender detection system using computer vision techniques. The system detects faces in real-time through a webcam feed and predicts the gender and age group of each detected face. It utilizes pre-trained deep learning models to perform the detection and classification tasks.

### Objective

The primary objective of this project is to demonstrate the application of computer vision and deep learning for real-time age and gender detection. The system aims to accurately identify the gender and approximate age group of individuals in the video stream.

### Methodology

The project follows these key steps:

1. **Face Detection**: Utilizes a pre-trained face detection model to locate faces within the webcam feed.

2. **Gender Classification**: For each detected face, extracts the facial region and feeds it into a pre-trained gender classification model. The model predicts whether the face belongs to a male or female.

3. **Age Estimation**: Alongside gender classification, the system estimates the approximate age group of each detected face. This is achieved by passing the facial region through a pre-trained age estimation model.

4. **Visualization**: Draws bounding boxes around detected faces and overlays text indicating the predicted gender and age group.

### Code Explanation

- The code starts by loading pre-trained models for face detection, gender classification, and age estimation.
- It then captures video frames from the webcam feed and processes them in real-time.
- For each frame, it detects faces using the face detection model and extracts the facial regions.
- The facial regions are fed into the gender and age estimation models to make predictions.
- Predicted gender and age group labels are displayed on the video frames along with bounding boxes around the detected faces.
- The system continues to process frames until the user quits by pressing 'q'.

### Dependencies

- OpenCV: For image and video processing.
- Pre-trained models:
  - Face detection: `opencv_face_detector.pbtxt`, `opencv_face_detector_uint8.pb`
  - Gender classification: `gender_deploy.prototxt`, `gender_net.caffemodel`
  - Age estimation: `age_deploy.prototxt`, `age_net.caffemodel`

### Conclusion

The age and gender detection system presented in this project showcases the capabilities of computer vision and deep learning in real-time applications. By accurately predicting the gender and approximate age group of individuals, the system can find applications in various domains, including retail analytics, audience analysis, and security systems. This project serves as a practical demonstration of how such systems can be implemented using readily available tools and pre-trained models.
