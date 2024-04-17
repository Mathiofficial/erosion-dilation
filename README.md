# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
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
<br>Erode the image

### Step5:
<br>Dilate the image

### Step6:
Display the output images

 
## Program:
### Erosion
``` python
import numpy as np
import cv2
import matplotlib.pyplot as plt
img1=np.zeros((100,400), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'Luffy',(5,70), font,2,(255),5,cv2.LINE_AA)
kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image_erode1=cv2.erode(img1,kernel1)
plt.imshow(image_erode1)
plt.axis("off")
```
### Dilation
```python
import numpy as np
import cv2
import matplotlib.pyplot as plt
img1=np.zeros((100,400), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'Luffy',(5,70), font,2,(255),5,cv2.LINE_AA)
kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image_dilate1=cv2.dilate(img1,kernel1)
plt.imshow(image_dilate1)
plt.axis("off")

```
## Output:

### Display the input Image

![Screenshot 2024-04-17 085656](https://github.com/Mathiofficial/erosion-dilation/assets/118787327/b0a24386-2c36-46e9-a18f-981b1e8e2fc8)

<br>

### Display the Eroded Image

![Screenshot 2024-04-17 085643](https://github.com/Mathiofficial/erosion-dilation/assets/118787327/67e5bc53-ef2a-43d6-858f-54c65ec8055f)

<br>

### Display the Dilated Image
![Screenshot 2024-04-17 085649](https://github.com/Mathiofficial/erosion-dilation/assets/118787327/07f63816-1946-44f2-aeba-b9d9a02f9629)


<br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
