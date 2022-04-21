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
image_1=cv2.imread("img1.jpg")
image_2=cv2.imread("img2.jpg")
cv2.imshow("pic1",image_1)
cv2.waitKey(0)
cv2.imshow("pic2",image_2)
cv2.waitKey(0)
  

```
ii) #To write the image
```
cv2.imwrite("pic_1.jpg",image_1)
cv2.imwrite("pic_2.jpg",image_2)


```
iii) #Find the shape of the Image
```python3
print(image_1.shape)
print(image_2.shape)


```
iv) #To access rows and columns

```python3
for i in range(70,90):
    for j in range(110,170):
        image_2[i][j]=[0,0,0]
cv2.imshow("pic_2",image_2)
cv2.waitKey(0)


```
v) #To cut and paste portion of image
```python3
image_1[200:220,110:175]=image_1[70:90,110:175]
cv2.imshow("pic_1",image_1)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image

<br>
![Screenshot (23)](https://user-images.githubusercontent.com/75234588/164487955-43108756-e764-4c7f-bdab-033cc82a284f.png)


![Screenshot (24)](https://user-images.githubusercontent.com/75234588/164487515-bc8e335d-541d-415c-9063-3dcf5cfba7e9.png)

<br>

### ii)Write the image

<br>![Screenshot (28)](https://user-images.githubusercontent.com/75234588/164487607-d8050bbc-de06-4c3b-b32d-d4275af9ceb4.png)

<br>

### iii)Shape of the Image

<br>![Screenshot (25)](https://user-images.githubusercontent.com/75234588/164487674-c32b3829-4f87-4f40-a092-a3b013cc138d.png)


<br>

### iv)Access rows and columns
<br>![Screenshot (26)](https://user-images.githubusercontent.com/75234588/164487720-76a375c4-e50f-4cb9-9c90-b9ad23c15298.png)

<br>

### v)Cut and paste portion of image
<br>![Screenshot (27)](https://user-images.githubusercontent.com/75234588/164487742-1acfd676-046c-404c-b7a1-81afc7b8b5b0.png)

<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


