# image-processing-lab

1.Develop a program to display grayscale image as tiny real and write program<br>
import cv2<br>
img1=cv2.imread('flower5.jpg',0)<br>
cv2.imshow('flower3',img1)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>

![image](https://user-images.githubusercontent.com/98301023/173814042-1f9fd68f-504c-42d3-b854-ff58bf7b027f.png)<br>
<br>


2.develop a program to display image to string using metaplotlib<br>
import matplotlib.image as mping<br>
import matplotlib.pyplot as plt<br>
img=mping.imread('flower5.jpg')<br>
plt.imshow(img)<br>

![image](https://user-images.githubusercontent.com/98301023/173814171-2a69155b-4f01-4945-a3ee-eae3aef6bca4.png)<br>



3.Develop program to perform linear transfermation rotation<br>
from PIL import Image<br>
img=Image.open("flower3.jpg")<br>
img=img.rotate(180)<br>
img.show()<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>

![image](https://user-images.githubusercontent.com/98301023/173815233-90a533a5-efb8-48e2-8a35-fc0b7b9761aa.png)<br>



4.develop a programt to convert color,string to RGB order value<br>
from PIL import ImageColor<br>
#using getrgb for yellow<br>
img1=ImageColor.getrgb("yellow")<br>
print(img1)<br>
#using getrgb for red<br>
img2=ImageColor.getrgb("red")<br>
print(img2)<br>

(255, 255, 0)<br>
(255, 0, 0)
<br>


5.write program to create image using color<br>
from PIL import Image<br>
img=Image.new('RGB',(200,400),(235,255,0))<br>
img.show()<br>

![image](https://user-images.githubusercontent.com/98301023/173815623-c11c4d89-1831-4ee0-a4c2-593f498fc683.png)<br>

<br>

6.develop a program to visualize the image using various color spaces<br>
import cv2<br>
import matplotlib.pyplot as plt<br>
import numpy as np<br>
img=cv2.imread("flower3.jpg")<br>
plt.imshow(img)<br>
plt.show()<br>
img=cv2.cvtColor(img,cv2.COLOR_BGR2RGB)<br>
plt.imshow(img)<br>
plt.show()<br>
img=cv2.cvtColor(img,cv2.COLOR_RGB2HSV)<br>
plt.imshow(img)<br>
plt.show()<br>
<br>
![image](https://user-images.githubusercontent.com/98301023/173815954-0de5ebd4-3533-46ba-a3f6-6ea6ccb27355.png)<br>

![image](https://user-images.githubusercontent.com/98301023/173816038-7a4d7d84-002b-47fe-8b06-b3fd613c21ee.png)<br>

![image](https://user-images.githubusercontent.com/98301023/173816088-5b584ac4-cbc8-47ed-96b1-1fb5c5c2e45b.png)<br>


<br>
7.write aprogram to display the image altribute <br>
from PIL import Image<br>
image=Image.open("flower5.jpg")<br>
print("Filename",image.filename)<br>
print("format",image.format)<br>
print("mode",image.mode)<br>
print("size",image.size)<br>
print("width",image.width)<br>
print("height",image.height)<br>
image.close()<br>


Filename flower5.jpg<br>
format JPEG<br>
mode RGB<br>
size (255, 132)<br>
width 255<br>
height 132<br>





#convert the original image to gray scale and then to to binary<br>
import cv2<br>
img=cv2.imread("plants2.jpg")<br>
print('original image length width',img.shape)<br>
cv2.imshow('original image',img)<br>

#to show resize image<br>
imgresize=cv2.resize(img,(150,160))<br>
cv2.imshow('resized image',imgresize)<br>
print('resized image length width',imgresize.shape)<br>
cv2.waitKey(0)<br>

OUTPUT
original image length width (751, 1000, 3)
resized image length width (160, 150, 3)

![image](https://user-images.githubusercontent.com/98301023/174042548-3d1ec7ff-8b7f-4add-8431-5125c716c172.png)<br>


resized image
![image](https://user-images.githubusercontent.com/98301023/174042760-0bc4c7da-374c-42a0-bd1e-ad6864fe8fc7.png)





#convert image to binary<br>
#read the image file<br>

img=cv2.imread('butterfly1.jpg')<br>

cv2.imshow("RGB",img)<br>

<br>


#grayscale<br>

img=cv2.imread("butterfly1.jpg",0)<br>

cv2.imshow("gray",img)<br>



#binary image<br>

ret,bw_img=cv2.threshold(img,127,255,cv2.THRESH_BINARY)<br>

cv2.imshow("binary",bw_img)<br>

cv2.waitKey(0)<br>

cv2.destroyAllWindows()<br>

OUTPUT
![image](https://user-images.githubusercontent.com/98301023/174045192-d8c64d61-cad7-4ebc-8640-54f776bb8ba9.png)<br>
![image](https://user-images.githubusercontent.com/98301023/174049390-d6114a69-30e3-4ff7-81f0-2d6e1e8e5b7b.png)<br>


![image](https://user-images.githubusercontent.com/98301023/174049599-4d11d4d7-6f00-479a-8edb-357df4388477.png)<br>





                     



