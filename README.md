# Green-Screen-Chroma-Key-Video-Effect
Create a green screen effect in a video using OpenCV.
import cv2
import numpy as np

cap = cv2.VideoCapture('greenscreen.mp4')
background = cv2.imread('background.jpg')

while True:
    ret, frame = cap.read()

    # Implement green screen effect logic

    cv2.imshow('Green Screen Effect', frame)

    if cv2.waitKey(1) & 0xFF == ord('q'):
        break

cap.release()
cv2.destroyAllWindows()
