## Image Color Space Analysis with OpenCV

**Description:**
This Python script, implemented in Jupyter Notebook format, loads a color image, converts it to the HSV color space, splits the HSV image into its components (hue, saturation, and intensity), displays the original image and its separated components, and finally saves the separated components as individual images. The script also provides download links for the saved images.

**Instructions:**
1. Ensure you have Python installed on your system along with the necessary libraries (OpenCV).
2. Download the provided image file named "shubham1.png" or replace it with your own image file.
3. Run the provided Python script in a Jupyter Notebook environment.
4. After running the script, the original image along with its HSV components (hue, saturation, and intensity) will be displayed.
5. The separated components will be saved as individual images named "hue.png", "saturation.png", and "intensity.png".
6. Download the saved images using the provided download links.

**Code:**
```python
# -*- coding: utf-8 -*-
import cv2
from google.colab.patches import cv2_imshow
from google.colab import files

# Load the color image
image = cv2.imread("shubham1.png")

# Convert the image to HSV
image_hsv = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)

# Split the HSV image into components
hue, saturation, intensity = cv2.split(image_hsv)

# Display the original image and the separated components
print("Original image:")
cv2_imshow(image)
print("HSV image:")
cv2_imshow(image_hsv)
print("Hue image:")
cv2_imshow(hue)
print("Saturation image:")
cv2_imshow(saturation)
print("Intensity image:")
cv2_imshow(intensity)

# Save the images
cv2.imwrite('hue.png', hue)
cv2.imwrite('saturation.png', saturation)
cv2.imwrite('intensity.png', intensity)

# Provide download links for the saved images
print("Download the Hue image:")
files.download('hue.png')
print("Download the Saturation image:")
files.download('saturation.png')
print("Download the Intensity image:")
files.download('intensity.png')
```
