### 📝 Proposed System
The proposed system leverages advanced **Computer Vision** and **Machine Learning** to monitor driver alertness in real-time. By analyzing facial expressions, eye movements, and yawning patterns, the system provides a robust safety layer. 

**Key Technical Workflow:**
*   **Face Detection:** Real-time video feed is processed using the **Haar-Cascade** algorithm for high-speed face detection.
*   **Eye Monitoring:** Utilizes **Eye Aspect Ratio (EAR)** to calculate the precise openness of the eyes.
*   **Yawn Detection:** Implements **Mouth Aspect Ratio (MAR)** to track lip distance and detect yawning.
*   **Smart Alerts:** When the system detects prolonged eye closure or frequent yawning, it triggers an auditory warning.

---

### 🏗️ Project Architecture
![System Architecture](architecture.jpg) 

---

### ⚙️ Working Steps
1.  **Environment Setup:** Integration of **OpenCV** for real-time image processing.
2.  **Facial Landmark Mapping:** Identifying 68 key points on the face using Dlib.
3.  **EAR Calculation:** Mathematical computation of eye openness.
4.  **Fatigue Analysis:** Simultaneous monitoring of mouth movements for yawning.
5.  **Drowsiness Validation:** Triggering state if EAR/MAR thresholds are breached.
6.  **Alert Mechanism:** Activation of a high-decibel auditory alert.

---

### 🖥️ Detection Framework
![Detection Framework](framework.jpg)

---

### 🚀 How to Run

1.  **Dependencies:**  
    Install all necessary libraries:  
    `pip install -r requirements.txt`

2.  **Landmark Predictor:**  
    Download `shape_predictor_68_face_landmarks.dat` and place it in the root folder.

3.  **Configuration:**  
    Update the `alert.wav` file path in `drowsiness_yawn.py`.

4.  **Execution:**  
    `python drowsiness_yawn.py`

---
