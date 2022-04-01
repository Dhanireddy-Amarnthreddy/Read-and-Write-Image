# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
```python
# Developed By:D.Amarnath REddy
# Register Number:212221240012
# To Read,display the image
import cv2
colorImage = cv2.imread('/Users/kodurusanathkumarreddy/Desktop/cars1.jpg',1)
cv2.imshow('212221240012-ReadingAndDisplaying',colorImage)
cv2.waitKey(0)



# To write the image
import cv2
colorImage = cv2.imread('/Users/kodurusanathkumarreddy/Desktop/cars1.jpg',1)
cv2.imwrite('/Users/kodurusanathkumarreddy/Desktop/written.jpg',colorImage)
written = cv2.imread('/Users/kodurusanathkumarreddy/Desktop/written.jpg',1)
cv2.imshow('212221240012-WrittenImage',written)
cv2.waitKey(0)
<br>
<br>




# Find the shape of the Image
import cv2
colorImage = cv2.imread('/Users/kodurusanathkumarreddy/Desktop/cars1.jpg',1)
print(colorImage.shape)



# To access rows and columns
import cv2
import random
colorImage = cv2.imread('/Users/kodurusanathkumarreddy/Desktop/cars1.jpg',1)
for i in range(100):
    for j in range(colorImage.shape[1]):
        colorImage[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221240012-AccessingRowsAndColumns',colorImage)
cv2.waitKey(0)




# To cut and paste portion of image
import cv2
colorImage = cv2.imread('/Users/kodurusanathkumarreddy/Desktop/cars1.jpg',1)
tag = colorImage[20:80,20:80]
colorImage[90:150,90:150] = tag
cv2.imshow('212221240012-CutAndPaste',colorImage)
cv2.waitKey(0)









```
## Output:

### i) Read and display the image

![](ReadDisplay.png)

<br>
<br>

### ii)Write the image
![](WrittenImage.png)


### iii)Shape of the Image
![](Shape1.png)


<br>
<br>

### iv)Access rows and columns
![](Accessing.png)
<br>
<br>

### v)Cut and paste portion of image
![](cutPaste.png)
<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


