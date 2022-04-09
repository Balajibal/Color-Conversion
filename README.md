# Color Conversion
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
 Convert BGR and RGB to HSV and GRAY

### Step2:
Convert HSV TO RGB AND BGR

### Step3:
Convert RGB and BGR to YCrCb

### Step4:
To Split and merge RGB Image

### Step5:
To Split and merge HSV Image

## Program:
```python
# Developed By: BALAJI N
# Register Number: 212220230006
# i) Convert BGR and RGB to HSV and GRAY
import cv2
goku = cv2.imread('goku.jpg')
modimg1 = cv2.cvtColor(goku,cv2.COLOR_BGR2HSV)
cv2.imshow('COLOR_BGR2HSV',modimg1)
cv2.waitKey(0)
modimg2 = cv2.cvtColor(goku,cv2.COLOR_RGB2HSV)
cv2.imshow('COLOR_RGB2HSV',modimg2)
cv2.waitKey(0)
modimg3 = cv2.cvtColor(goku,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',modimg3)
cv2.waitKey(0)
modimg4 = cv2.cvtColor(goku,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',modimg4)
cv2.waitKey(0)





# ii)Convert HSV to RGB and BGR
modimg5 = cv2.cvtColor(goku,cv2.COLOR_HSV2BGR)
cv2.imshow('COLOR_RGB2HSV',modimg5)
cv2.waitKey(0)
modimg6 = cv2.cvtColor(goku,cv2.COLOR_HSV2RGB)
cv2.imshow('COLOR_HSV2RGB',modimg6)
cv2.waitKey(0)





# iii)Convert RGB and BGR to YCrCb
modimg7 = cv2.cvtColor(goku,cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGB2YCrCb',modimg7)
cv2.waitKey(0)
modimg8 = cv2.cvtColor(goku,cv2.COLOR_BGR2YCrCb)
cv2.imshow('RCB2YCrCb',modimg8)
cv2.waitKey(0)




# iv)Split and Merge RGB Image
red = image[:,:,0]
green = image[:,:,1]

blue = image[:,:,2]


Merge:
cv2.merge((blue,green,red))



# v) Split and merge HSV Image
hsv_image = cv2.cvtColor(goku, cv2.COLOR_BGR2HSV)
h, s, v = cv2.split(hsv_image)
s.fill(255)
v.fill(255)
hsv_image = cv2.merge([h, s, v])

cv2.imshow('example', hsv_image)
cv2.waitKey()




```
## Output:
### i) Original Image
![goku](https://user-images.githubusercontent.com/75234946/162558259-a5743cd3-d94c-4b6c-abc9-71a68af11e47.jpg)

### ii) BGR and RGB to HSV and GRAY
![Screenshot (38)](https://user-images.githubusercontent.com/75234946/162558272-a82e78b0-0b25-46a8-8f2e-774c1f1f5e0b.png)
![Screenshot (37)](https://user-images.githubusercontent.com/75234946/162558338-028d7478-01aa-497d-83ae-beb5ad6c63d9.png)
![Screenshot (49)](https://user-images.githubusercontent.com/75234946/162558362-8cff74af-d774-4611-9626-8156a7bb2afb.png)
![Screenshot (41)](https://user-images.githubusercontent.com/75234946/162558401-f827e0a5-8d6d-4b42-85e3-96818372584e.png)




### iii) HSV to RGB and BGR
![Screenshot (44)](https://user-images.githubusercontent.com/75234946/162558425-77ab34a5-d7be-4f2b-b09d-06f4001797dd.png)
![Screenshot (50)](https://user-images.githubusercontent.com/75234946/162558472-4cf3128c-a3f0-42e9-9b1c-23532a558fc7.png)



### iv) RGB and BGR to YCrCb
![Screenshot (53)](https://user-images.githubusercontent.com/75234946/162558493-101246b7-8645-4685-be41-9e0095357011.png)
![Screenshot (51)](https://user-images.githubusercontent.com/75234946/162558539-8a4d153a-d82f-4361-90e7-5b796411fc95.png)



### v) Split and merge RGB Image
![Screenshot (54)](https://user-images.githubusercontent.com/75234946/162558560-c7db04cf-6e50-4347-a297-2d18ec15d15f.png)


### vi) Split and merge HSV Image
![Screenshot (55)](https://user-images.githubusercontent.com/75234946/162558585-d4d0b532-cfc4-4fae-b115-22d45d15fa06.png)



## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
