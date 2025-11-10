# WORKSHOP-3-Canny-Edge-Detection

# Name : K.SRISARAN KARTHIK
# Reg No : 212224230275


# CODE :
```
import cv2
import matplotlib.pyplot as plt
# Read the image
img = cv2.imread('photo1.jpg',cv2.IMREAD_GRAYSCALE)
# Apply Gaussian blur to reduce noise
blurred =cv2.GaussianBlur(img, (5,5),0)
# Detect edges using Canny
edges = cv2.Canny(blurred, 50, 150) #Adjust threshold values as needed
# Plot the original image and the detected edges
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()

```
# OUTPUT :

<img width="1011" height="537" alt="image" src="https://github.com/user-attachments/assets/c46ec1a7-1d54-4ba1-8363-b3a44c1a382e" />

