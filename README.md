# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import cv2 and numpy packages.
### Step2:
Create the text using cv2.putText() and show the Imge containing Text.
### Step3:
Create the structuring element using cv2.getStructuralElement().

### Step4:
Using structuring element erode the image.

### Step5:
Usig structuring element dilate the image.

### Step6:
Show the Erroded and Dilated Images with Original Image.
## Program:

``` Python
# Import the necessary packages
import cv2
import numpy as np

# Create the Text using cv2.putText
font=cv2.FONT_HERSHEY_SCRIPT_SIMPLEX
cv2.putText(img1,'Pavan',(5,50),font,2,(255),3,cv2.LINE_AA)
cv2.imshow('My Image',img1)

# Create the structuring element
kernel1=cv2.getStructuringElement(cv2.MORPH_ELLIPSE,(7,7))

# Erode the image
erodeimg=cv2.erode(img1,kernel1)
cv2.imshow("Eroded Image",erodeimg)

# Dilate the image
dilateimg=cv2.dilate(img1,kernel1)
cv2.imshow("Dilated Image",dilateimg)


```
## Output:

### Display the input Image

![EX9 1](https://user-images.githubusercontent.com/94827772/169644408-cba83aab-2fb5-47b2-8ebe-1f39b8b2508d.png)
</br>
### Display the Eroded Image
![EX9 2](https://user-images.githubusercontent.com/94827772/169644424-860d3776-8e8a-4340-a771-563abff8d339.png)
</br>
### Display the Dilated Image
![EX9 3](https://user-images.githubusercontent.com/94827772/169644454-cd6b5333-57c6-4291-92c2-aa5b282af172.png)
</br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
