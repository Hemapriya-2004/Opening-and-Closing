# Opening-and-Closing

## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.



### Step2:
Create the Text using cv2.putText


### Step3:
Create the structuring element.


### Step4:
Use Opening operation.


### Step5:
Use Closing Operation.


 
## Program:

/*
Developed by   : R.HEMA PRIYA
Register Number: 212220230036
*/
``` Python
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
img=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img,'Hema Priya',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img)
plt.show()

# Create the structuring element
kernel=cv2.getStructuringElement(cv2.MORPH_RECT,(9,9))

# Use Opening operation
image_open=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)
plt.axis('off')
plt.imshow(image_open)
plt.show()

# Use Closing Operation
image_close=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)
plt.axis('off')
plt.imshow(image_close)
plt.show()




```
## Output:

### Display the input Image

![image](https://user-images.githubusercontent.com/94184828/174797944-4a472b80-d9b9-408c-abc5-183ffad07c18.png)

### Display the result of Opening
![image](https://user-images.githubusercontent.com/94184828/174798029-10fa3441-44c2-4f00-8fa0-928fbe20b2b5.png)


### Display the result of Closing
![image](https://user-images.githubusercontent.com/94184828/174798090-a8aee47a-7b67-4413-a4d3-94c5af17ea94.png)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
