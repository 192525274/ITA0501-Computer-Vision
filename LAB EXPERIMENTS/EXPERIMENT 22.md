## PROGRAM
``` PYTHON
import cv2
import numpy as np
image = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
kernel = np.ones((5,5), np.uint8)
closed_image = cv2.morphologyEx(gray_image, cv2.MORPH_CLOSE, kernel)
cv2.imshow('Original Image', image)
cv2.imshow('Closed Image', closed_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT
<img width="959" height="502" alt="image" src="https://github.com/user-attachments/assets/4ccfea3f-2141-4d36-9435-04cdf788474c" />
<img width="959" height="504" alt="image" src="https://github.com/user-attachments/assets/50a24f12-9e3b-44b6-ad19-ed070acfe1ee" />


