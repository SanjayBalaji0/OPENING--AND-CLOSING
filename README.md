# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
<br>Import the necessary packages
### Step2:
<br>Create the Text using cv2.putText
### Step3:
<br>Create the structuring element
### Step4:
<br>Use Opening operation
### Step5:
<br>Use Closing Operation

 
## Program:
```
Name: Sanjay Balaji S
REg. No: 212223240149
```

### OPENING
``` python
import numpy as np
import cv2
import matplotlib.pyplot as plt
img1=np.zeros((100,400), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'SanjayBalaji',(5,70), font,2,(255),5,cv2.LINE_AA)
kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image1=cv2.morphologyEx(img1,cv2.MORPH_OPEN,kernel)
plt.imshow(image1)
plt.axis("off")

```
### CLOSING
```python
import numpy as np
import cv2
import matplotlib.pyplot as plt
img1=np.zeros((100,400), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'SanjayBalaji',(5,70), font,2,(255),5,cv2.LINE_AA)
kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image2=cv2.morphologyEx(img1,cv2.MORPH_CLOSE,kernel)
plt.imshow(image2)
plt.axis("off")
```
## Output:
### Display the result of Opening
![image](https://github.com/user-attachments/assets/f6ea6086-d12f-4758-a819-01097494a66b)



### Display the result of Closing
![image](https://github.com/user-attachments/assets/ed3d8da7-c7b4-49a1-96e4-b98cd882dfb0)




## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
