# H1 ABSTRACT

Sign language serves as a crucial mode of communication for the deaf and hard- of-hearing community, yet barriers in communication with the hearing population persist. This project presents a Sign Language Recognition System utilising machine learning techniques to bridge this gap, enhancing accessibility and inclusivity.Key features include high recognition accuracy, real-time processing, and an intuitive user interface that supports seamless interaction. The implementation showcases the potential of machine learning in advancing assistive technologies, offering a practical solution to improve communication for the deaf and hard-of-hearing community. Future enhancements aim to incorporate advanced deep learning algorithms and expand the gesture database to cover more sign languages and dialects, further increasing the system’s utility and reach.This project introduces a Sign Language Recognition System leveraging machine learning frameworks such as TensorFlow and Scikit Learn to mitigate these challenges and promote inclusivity. Instead of convolutional neural networks, the system employs MediaPipe, a robust framework for real-time hand and body motion tracking, to interpret and translate sign language gestures into textual or spoken language in real-time. Trained on an extensive dataset of various sign languages and gestures, the model demonstrates adapt- ability accommodating different users and contexts.

## H2 Block Diagram
The system for Sign Language Recognition (SLR) is meticulously designed using a robust combination of technologies. Initially, the system employs a camera to capture live video feeds of sign language gestures, facilitated by OpenCV for seamless webcam access. These video frames are processed in real-time using MediaPipe, which detects and draws landmarks on the hands and body. MediaPipe extracts key points from each frame, representing the positions and movements of the fingers and hands.
During the training phase, these key points are collected and stored as training data, annotated with corresponding labels that signify different sign language gestures. This data undergoes preprocessing using Sci-Kit Learn, involving tasks such as normalisation and feature selection. Subsequently, TensorFlow is utilised to construct and train a neural network model specifically tailored for SLR. The neural network learns to classify gestures based on the patterns present in the key points data.
In the testing phase, the system again captures live video feeds through the camera and processes them with MediaPipe to detect landmarks and extract key points. These key points, now serving as testing data, are fed into the same neural network model trained earlier. The model classifies the gestures based on the learned patterns.
The final step involves evaluating the model’s performance. The system compares the model’s predictions with the actual labels of the test data to determine accuracy. Performance metrics such as accuracy, precision.This comprehensive approach ensures a robust and efficient SLR system capable of real-time gesture tracking and precise interpretation.

