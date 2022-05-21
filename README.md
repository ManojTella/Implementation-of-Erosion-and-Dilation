# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages to do Erosion and Dilution.
<br>


### Step2:
Create the text image of our name using putText from cv2 package.
<br>

### Step3:
Create the required structural element.
<br>

### Step4:
Apply Erode and Dilution for our NameImage.
<br>

### Step5:
Display the output images.
<br>

### Step6:
End the program.
<br>

 
## Program:
### Developed By: Manoj Guna Sundar Tella.
### Register Number: 212221240026.

``` 
# Import the necessary packages

import cv2
import numpy


# Create the Text using cv2.putText

NameImage = numpy.zeros((100,1000),dtype='uint8')
font = cv2.FONT_HERSHEY_SCRIPT_COMPLEX
cv2.putText(NameImage,'Manoj Guna Sundar Tella.',(50,70),font,2,(255),5,cv2.LINE_4)
cv2.imshow("Name Image",NameImage)



# Create the structuring element

kernel1 = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))



# Erode the image

erodeImage = cv2.erode(NameImage,kernel1)



# Dilate the image


dilationImage = cv2.dilate(NameImage,kernel1)

# Displaying the image
cv2.imshow("Name Image",NameImage)
cv2.imshow("Erode Image",erodeImage)
cv2.imshow("Dilated Image",dilationImage)
```
## Output:

### Display the input Image
![dip1](https://user-images.githubusercontent.com/94883876/169644352-c18d8c99-e5d4-40e0-b7fd-f4064a583d90.png)

<br>
<br>
<br>
<br>
<br>
<br>

### Display the Eroded Image
![dip2](https://user-images.githubusercontent.com/94883876/169644360-17001c41-8ea4-4bab-a005-924105864d5c.png)

<br>
<br>
<br>
<br>
<br>
<br>

### Display the Dilated Image
![dip3](https://user-images.githubusercontent.com/94883876/169644461-3db51096-0925-4410-829d-89161da9b710.png)

<br>
<br>
<br>
<br>
<br>
<br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
