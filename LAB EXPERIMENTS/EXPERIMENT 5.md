## PROGRAM
```PYTHON
import cv2 
image = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY) 
cv2.imshow("Original Image", image) 
cv2.imshow("Grayscale Image", gray_image) 
cv2.waitKey(0) 
cv2.destroyAllWindows() 
```
# OUTPUT
<img width="959" height="502" alt="image" src="https://github.com/user-attachments/assets/74c0db25-8dc1-4f63-8d15-13957631d9c6" />
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/dd69c0dc-c74a-4cf0-aff6-00651f5e4e86" />


