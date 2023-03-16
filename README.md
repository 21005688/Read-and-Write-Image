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
### Developed By:
### Register Number: 
i) #To Read,display the image
```
import cv2
color= cv2.imread('flo.JPG',1)
cv2.imshow('DEEPIKA212221230016',color)
cv2.waitKey(0)
  

```
ii) #To write the image
```
import cv2
color= cv2.imread('flo.JPG',-1)
cv2.imwrite('flo.JPG',color)



```
iii) #Find the shape of the Image
```
import cv2
color=cv2.imread('flo.JPG',1)
print(color.shape)



```
iv) #To access rows and columns

```
import cv2
import random
img= cv2.imread('flo.JPG',-1)
for i in range(150):
    for j in range(img.shape[1]):
        img[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('DEEPIKA212221230016',img)
cv2.waitKey(0)



```
v) #To cut and paste portion of image
```
import cv2
img1=cv2.imread('flo.JPG',-1)
copied_portion=img1[10:60,10:120]
img1[110:160,110:220]=copied_portion
cv2.imshow('DEEPIKA212221230016',img1)
cv2.waitKey(0)
cv2.destroyAllWindows()



```

## Output:

### i) Read and display the image

![I-1](https://user-images.githubusercontent.com/94747031/225486667-aee5bb59-0f9a-479f-9fc9-fdf7d55a872e.png)


### ii)Write the image

![i-4](https://user-images.githubusercontent.com/94747031/225486809-3883abaa-0210-49ef-899c-039a6fb437b5.png)


### iii)Shape of the Image


![i-5](https://user-images.githubusercontent.com/94747031/225486831-f039558e-f55b-4391-b217-737fad0e3217.png)

### iv)Access rows and columns

![i-2](https://user-images.githubusercontent.com/94747031/225486848-caad9ed8-613c-40f3-9acc-dc56b2dff2e3.png)

### v)Cut and paste portion of image

![i-3](https://user-images.githubusercontent.com/94747031/225486877-b78f3eae-d64f-4327-ae5e-903d929c0d05.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


