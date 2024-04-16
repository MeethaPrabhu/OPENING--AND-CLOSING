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
### OPENING
``` python
import numpy as np
import cv2
import matplotlib.pyplot as plt
img1=np.zeros((100,400), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'Engineer',(5,70), font,2,(255),5,cv2.LINE_AA)
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
cv2.putText(img1,'Engineer',(5,70), font,2,(255),5,cv2.LINE_AA)
kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image2=cv2.morphologyEx(img1,cv2.MORPH_CLOSE,kernel)
plt.imshow(image2)
plt.axis("off")
```
## Output:

### Display the input Image
<br>![image](https://github.com/MeethaPrabhu/OPENING--AND-CLOSING/assets/119401038/cd0aa95d-87f6-4422-89e2-3c2999b50be1)


### Display the result of Opening
<br>![image](https://github.com/MeethaPrabhu/OPENING--AND-CLOSING/assets/119401038/de17c5c1-c221-4d0f-9006-ee012755eb45)



### Display the result of Closing
<br>![Uploading image.png…]()



## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
