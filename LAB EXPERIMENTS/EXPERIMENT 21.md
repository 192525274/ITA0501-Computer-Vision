## PROGRAM
```PYTHON
import cv2
import numpy as np
image = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
kernel = np.ones((5,5), np.uint8)
opened_image = cv2.morphologyEx(gray_image, cv2.MORPH_OPEN, kernel)
cv2.imshow('Original Image', image)
cv2.imshow('Opened Image', opened_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/95943e18-25be-429d-839e-70fc9a86a739" />
<img width="959" height="502" alt="image" src="https://github.com/user-attachments/assets/e79c6391-5b61-434f-b1ec-768f2c167026" />



