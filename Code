
"""Untitled5.ipynb
import cv2

Load the color image

image = cv2.imread("shubham1.png")

Convert the image to HSV

image_hsv = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)

Split the HSV image into components

hue, saturation, intensity = cv2.split(image_hsv)

Display the original image and the separated components

print("original image")
cv2_imshow(image)
print("hsv image")
cv2_imshow(image_hsv)
print("hue image")
cv2_imshow(hue)
print("saturation image")
cv2_imshow(saturation)
print("intensity image")
cv2_imshow(intensity)

Save the images

cv2.imwrite('hue.png', hue)
cv2.imwrite('saturation.png', saturation)
cv2.imwrite('intensity.png', intensity)
#Provide download links for the saved images
print("Download the Hue image:")
files.download('hue.png')
print("Download the Saturation image:")
files.download('saturation.png')
print("Download the Intensity image:")
files.download('intensity.png')
