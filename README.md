HOMEWORK 1
After the installation of Anaconda, Jupyter Notebook, and the required virtual environment, you will have to test that everything has been set up correctly. For that purpose, you will have to execute the following code and run it without errors.

The code loads an image and creates a picture collage consisting of 4 pictures. Each of the four pictures is a version of the original image with the colour channels swapped.

You will also have to also finish some part of the code :-)

import cv2
import numpy as np
from matplotlib import pyplot as plt
plt.rcParams['figure.figsize'] = [15, 10]
# Load an image (you can freely chose any image you like)
img = 
# Convert it to RGB
img = 
# Plot it
plt.imshow(img)
Let's make a collage.

# Split the image into the three colour channels
red, green, blue = cv2.split(img)

# Compose the image in the RGB colour space
img1 = cv2.merge([red, green, blue])

# Compose the image in the RBG colour space
img2 = 

# Compose the image in the GRB colour space
img3 = 

# Compose the image in the BGR colour space
img4 =

# Create the collage
out1 = np.hstack([img1, img2])
out2 = np.hstack([img3, img4])
out = np.vstack([out1, out2])

# Plot the collage
plt.imshow(out)
plt.axis(False)
And now you are going to make a simple geometric collage. You need to flip your image both horizontally and vertically to obtain the following result.

alt text

You can flip the images "manually" but you might also find useful the numpy functions fliplr and flipud ;-).

# Load an image (you can freely chose any image you like)
img = 
# Convert it to RGB
img = 

# Make a collage


# Plot the collage