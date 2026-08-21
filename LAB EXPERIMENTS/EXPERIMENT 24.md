## PROGRAM
```PYTHON
import cv2
import numpy as np
# Read the image
image = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
# Define a kernel (5x5 structuring element)
kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))
# Apply the Black Hat transformation
blackhat = cv2.morphologyEx(image, cv2.MORPH_BLACKHAT, kernel)
# Display images
cv2.imshow("Original Image", image)
cv2.imshow("Black Hat Image", blackhat)
# Wait for a key press and close the windows
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/309ce5b8-767b-49a7-a055-e5c0fd98299c" />
<img width="959" height="502" alt="image" src="https://github.com/user-attachments/assets/fc583907-8cca-4352-acd9-3e5e56bc8e77" />


