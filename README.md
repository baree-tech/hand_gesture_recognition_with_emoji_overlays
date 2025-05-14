# Hand Gesture Recognition with Emoji Overlays

This project implements real-time hand gesture recognition using MediaPipe and OpenCV in Python. It detects specific hand gestures like "Thumbs Up" and "Victory Sign" from a webcam or video file and displays animated responses such as emojis and fireworks.
**Features**

- Real-time hand tracking using MediaPipe.
- Detects:
  - *Thumbs Up*: Triggers a LIKE emoji.
  - *Victory Sign*: Triggers a fireworks animation.
- Overlay PNG emojis with transparency on video frames.
- Record output to a video file.

**Demo**

- LIKE gesture displays a thumbs-up emoji.
- Victory gesture shows animated fireworks.
- Emoji overlays are dynamically positioned.
- Output can be recorded as my_gesture_video.mp4.

**Installation**

bash
pip install opencv-python mediapipe numpy

**Usage**

	1.	Place like.png and fireworks.png in the project directory.
	2.	Run the Python script:

handgesture.ipynb


	3.	To use a video file instead of a webcam, modify this line:

cap = cv2.VideoCapture('your_video.mp4')


**File Structure**
	•	handgesture.ipynb: Main code file.
	•	like.png: Emoji image for thumbs-up.
	•	fireworks.png: Fireworks overlay image.
	•	my_gesture_video.mp4: Output video (if enabled).

**How It Works**
	•	MediaPipe provides 21 landmark coordinates for each hand.
	•	The code calculates:
	•	Thumb angle to detect thumbs-up.
	•	Y-position of fingertips relative to joints for finger count.
	•	Detected gestures trigger visual effects using image overlays.

**Future Ideas**
	•	Add more gesture types (OK, Heart, Rock, etc.).
	•	Integrate with sound effects or GUI.
	•	Extend for virtual interaction or games.

**License**

Open for educational and non-commercial use.

⸻

Created by Bareera Mushthak
linkedIn : linkedin.com/in/bareera-mushthak


---
