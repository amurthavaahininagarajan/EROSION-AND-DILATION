##  EROSION-AND-DILATION

## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.
<br>


### Step2:
Create the text image using cv2.putText.
<br>

### Step3:
Then create the structuring image for dilation/erosion.
<br>

### Step4:
Apply erosion and dilation using plt.erode and plt.dilate.
<br>

### Step5:
Plot the images using plt.imshow.
<br>

 
## Program:
```
Developed by: Amurtha vaahini.KN
Register number:212222240008
```


# Import the necessary packages:
```
import numpy as np
import cv2
import matplotlib.pyplot as plt
```



# Create the Text using cv2.putText:
```
image = np.zeros((100,500),dtype = 'uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(image,"AMURTHA VAAHINI",(5,70),font,2,(255),5,cv2.LINE_AA)
plt.imshow(image,cmap='gray')
plt.title('Input Text'), plt.xticks([]), plt.yticks([])
plt.show()
```



# Create the structuring element:
```
kernel=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
```



# Erode the image:
```
image_erode=cv2.erode(image,kernel)
plt.imshow(image_erode,cmap='gray')
plt.title('Eroded Text'), plt.xticks([]), plt.yticks([])
plt.show()
```




# Dilate the image:
```
image_dilate=cv2.dilate(image,kernel)
plt.imshow(image_dilate,cmap='gray')
plt.title('Dilated Text'), plt.xticks([]), plt.yticks([])
plt.show()
```





## Output:

### Display the input Image:
![1](https://github.com/amurthavaahininagarajan/EROSION-AND-DILATION/assets/118679102/7ae2570f-d3d4-4a83-aa23-cfa610878133)



<br>
<br>
<br>
<br>
<br>
<br>

### Display the Eroded Image:
![2](https://github.com/amurthavaahininagarajan/EROSION-AND-DILATION/assets/118679102/088be846-bd21-4b3a-b03f-692129f62013)


<br>
<br>
<br>
<br>
<br>
<br>

### Display the Dilated Image:


![3](https://github.com/amurthavaahininagarajan/EROSION-AND-DILATION/assets/118679102/ee18bb6f-c8cb-41ba-8cca-2f33465214bc)


<br>
<br>
<br>
<br>
<br>
<br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
