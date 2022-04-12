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
# Developed By:
Srinivasan S

# Register Number:
212220230048

# To Read,display the image
import cv2
panda_img = cv2.imread('panda.jpg',1)
cv2.imshow('panda',panda_img)
cv2.waitKey(0)
destroyAllWindows()


# To write the image
import cv2
panda_img = cv2.imread('panda.jpg',1)
cv2.imwrite('new image.jpg',panda_img)



# Find the shape of the Image
import cv2
panda_img = cv2.imread('panda.jpg',1)
print(panda_img.shape))



# To access rows and columns
import random
for i in range(100):
    for j in range(panda_img.shape[1]):
        panda_img[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('Panda',panda_img)
cv2.waitKey(0)
destroyAllWindows()



# To cut and paste portion of image
import cv2
panda_img = cv2.imread('panda.jpg',-1)
tag = panda_img[300:400,300:400]
panda_img[50:150,50:150] = tag
cv2.imshow('Panda',panda_img)
cv2.waitKey(0)
destroyAllWindows()








```
## Output:

### i) Read and display the image
![Screenshot 2022-04-12 193802](https://user-images.githubusercontent.com/103049243/162981244-3c9166d5-162b-4d80-ac96-22fff9b3bba8.png)
<br>
<br>

### ii)Write the image
![Screenshot 2022-04-12 193923](https://user-images.githubusercontent.com/103049243/162981433-01c0bd48-e2b5-452c-8f43-c515704c5256.png)
<br>
<br>

### iii)Shape of the Image

<br>![Screenshot 2022-04-12 194046](https://user-images.githubusercontent.com/103049243/162981717-3e7fab2f-9dc6-451b-9405-ea74968d915e.png)

<br>

### iv)Access rows and columns
![Screenshot 2022-04-12 194153](https://user-images.githubusercontent.com/103049243/162981955-70d14e67-893b-4617-a0d9-08033b24d902.png)
<br>
<br>

### v)Cut and paste portion of image
![Screenshot 2022-04-12 194255](https://user-images.githubusercontent.com/103049243/162984055-67865230-d7e0-4a2d-b2c3-980343eed9f1.png)
<br>
<br>


## Result:

Thus the images are read, displayed, and written successfully using the python program.
