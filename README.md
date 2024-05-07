# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages

### Step2
Create the Text using cv2.putText

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

## Program:
```
Developed by: ROHITH
Register Number: 212222230121
```
### Display the input Image
```python
import cv2
import numpy as np

img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'ROHITH', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)
```
### Create ths structured element
```python
struct_ele = np.ones((9, 9), np.uint8)
```
### Display the result of Opening
```python
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)
```
### Display the result of Closing
```python
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)
```
## Output:

### Display the input Image

![Screenshot 2024-05-07 235109](https://github.com/Rohithravi333/OPENING--AND-CLOSING/assets/119394126/dcff56f8-9083-49e8-bb4b-4605c065f095)


### Display the result of Opening

![Screenshot 2024-05-07 235241](https://github.com/Rohithravi333/OPENING--AND-CLOSING/assets/119394126/53f6cc2d-3416-4fd1-aa53-13c060cbf74e)


### Display the result of Closing
![Screenshot 2024-05-07 235308](https://github.com/Rohithravi333/OPENING--AND-CLOSING/assets/119394126/949b680a-6b99-4788-b3f7-8481a87f07fc)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
