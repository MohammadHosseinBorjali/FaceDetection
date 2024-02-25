# FaceDetection

 **README for main_video.py**

**Description:**

This Python script utilizes a webcam to detect and recognize faces in real-time, displaying their names on the screen.

**Installation Requirements:**

- Python 3
- OpenCV (`cv2`) library: `pip install opencv-python`
- SimpleFacerec library: `pip install simple-facerec`

**Prerequisites:**

- Ensure a folder named "images" is present within the same directory as the script, containing pre-saved images of individuals for recognition.

**Instructions to Run:**

1. Navigate to the script's directory using a terminal.
2. Execute the script: `python main_video.py`

**Functionality:**

- **Encode faces:** The script automatically encodes faces from images within the "images" folder for recognition.
- **Load camera:** The script accesses your webcam.
- **Real-time detection and recognition:** The script continuously analyzes video frames from the webcam.
  - Detect faces within the frames.
  - Recognize known faces by comparing them to the encoded images.
  - Draw rectangles around detected faces.
  - Display the corresponding names above each rectangle.
- **Exit:** Press the Esc key (`key == 27`) to terminate the script.

**Troubleshooting:**

- **Missing libraries:** If you encounter errors regarding missing libraries, install them using `pip` as mentioned in the Installation Requirements.
- **Webcam issues:** Ensure your webcam is functional and accessible.
- **Face recognition difficulties:**
  - Verify that images in the "images" folder are adequately illuminated and clearly show individuals' faces.
  - Reposition yourself for clearer recognition if faces are not properly detected.

**Additional Information:**

- Explore the SimpleFacerec library for further customization and configuration options.
