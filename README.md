📝 Proposed System
The proposed system leverages advanced Computer Vision and Machine Learning to monitor driver alertness in real-time. By analyzing facial expressions, eye movements, and yawning patterns, the system provides a robust safety layer.
Key Technical Workflow:
Face Recognition: Real-time video feed is processed using the Haar-Cascade algorithm for high-speed face detection.
Eye Monitoring: Utilizes Eye Aspect Ratio (EAR) to calculate the precise openness of the eyes.
Yawn Detection: Implements Mouth Aspect Ratio (MAR) to track lip distance and detect yawning.
Smart Alerts: When the system detects prolonged eye closure or frequent yawning (falling below a specific threshold), it triggers an auditory warning to alert the driver.
⚙️ Working Steps
Environment Setup: Integration of OpenCV for real-time image processing.
Facial Landmark Mapping: Applying algorithms to identify 68 key points on the face (eyes, mouth, nose).
EAR Calculation: Real-time mathematical computation of eye openness.
Fatigue Analysis: Simultaneous monitoring of mouth movements for yawning.
Drowsiness Validation: If the EAR remains below the threshold for a pre-defined duration, the system confirms a state of drowsiness.
Alert Mechanism: Activation of a high-decibel auditory alert to regain the driver’s focus.
🚀 How to Run
Dependencies: Install all necessary libraries using:
pip install -r requirements.txt
Landmark Predictor: Download the shape_predictor_68_face_landmarks.dat file from here and place it in the project root folder.
Configuration: Update the file path for alert.wav in the drowsiness_yawn.py script.
Execution: Run the main application:
python drowsiness_yawn.py
