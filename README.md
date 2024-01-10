# Gesture_control
I used mediapipe to detect hand landmarks on my hand from the camera. I saved different hand landmark coordinates based on the hand gestures for my training data. Hand gestures: palm, fist, like sign, dislike sign, fist with straight index and middle finger.
Link to the website fo mediapipe: https://developers.google.com/mediapipe/solutions/vision/hand_landmarker
The hand_model prepares the training data to machine learning and trains different models. I compared a logistic regression model and a decision tree model. The logistic regression model was 99% accurate while the decision tree was 96% accurate. I also saved the logistic regression to pickle as 2024_stemsisters_project.pickle.
The hand_gesture_recogniser saves the image from the camera, and draws the skeleton to the hand. With the model I trained it predicts the hand gesture and based on the gesture it controls my mouse.
Palm: Move the mouse if palm is moved!
Fist: Stay!
Like sign: Scroll up!
Dislike sign: Scroll down!
Fist with straight index and middle finger: Click with the left part of the mouse!
