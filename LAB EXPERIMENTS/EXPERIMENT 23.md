## PROGRAM
``` PYTHON
import cv2
import numpy as np
image = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
kernel = np.ones((5,5), np.uint8)
top_hat_image = cv2.morphologyEx(gray_image, cv2.MORPH_TOPHAT, kernel)
cv2.imshow('Original Image', image)
cv2.imshow('Top Hat Image', top_hat_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/670d97c8-d68c-48cf-9aa1-07ba3dc68dca" />
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/d8cd350e-225b-44be-b4b3-e13f5e8bdb58" />



