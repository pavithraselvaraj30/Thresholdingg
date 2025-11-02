# THRESHOLDING
## Aim
To segment the image using global thresholding, adaptive thresholding and Otsu's thresholding using python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Algorithm

### Step1:
Load the necessary packages

### Step2:

Read the image and convert to grayscale 
### Step3:

Use global thresholding to segment the image.

### Step4:

Use Adaptive thresholding to segment the image.

### Step5:
Use Otsu's method to segment the image and display the results.

## Program
# NAME:PAVITHRA S
# REG.NO:212223230147
```
# Load the necessary packages

import cv2
import numpy as np
import matplotlib.pyplot as plt


# Read the Image and convert to grayscale

image = cv2.imread("/content/cat.jpeg")  # Replace with your image file path
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)  # Convert to grayscale
plt.subplot(2, 2, 1)
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))  # Convert from BGR to RGB for display
plt.title("Original Image")
plt.axis('off')


# Display the results
# Global Thresholding
plt.subplot(2, 2, 2)
plt.imshow(global_thresholded, cmap='gray')
plt.title("Global Thresholding")
plt.axis('off')

# Adaptive Thresholding
plt.subplot(2, 2, 3)
plt.imshow(adaptive_thresholded, cmap='gray')
plt.title("Adaptive Thresholding")
plt.axis('off')

# Otsu's Method
plt.subplot(2, 2, 4)
plt.imshow(otsu_thresholded, cmap='gray')
plt.title("Otsu's Method")
plt.axis('off')

# Show the plot
plt.tight_layout()
plt.show()
```


## Output

### Original Image
<img width="435" height="291" alt="Screenshot 2025-11-02 133940" src="https://github.com/user-attachments/assets/db0849ae-71be-4ab7-bad2-cd8d022007b8" />


### Global Thresholding
<img width="434" height="288" alt="Screenshot 2025-11-02 133951" src="https://github.com/user-attachments/assets/7281166f-4c76-4d3e-8500-883d2202f456" />


### Adaptive Thresholding
<img width="426" height="293" alt="Screenshot 2025-11-02 133958" src="https://github.com/user-attachments/assets/a8e40716-d267-49ae-87e7-7786f3b7b900" />


### Optimum Global Thesholding using Otsu's Method
<img width="473" height="290" alt="Screenshot 2025-11-02 134008" src="https://github.com/user-attachments/assets/069b8baa-6b13-4f1d-bac1-46177b35f7e0" />



## Result
Thus the images are segmented using global thresholding, adaptive thresholding and optimum global thresholding using python and OpenCV.
