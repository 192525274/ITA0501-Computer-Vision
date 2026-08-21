## PROGRAM
``` PYTHON
import cv2
# Read the image
image = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
bigger_image = cv2.resize(image, None, fx=2, fy=2, interpolation=cv2.INTER_LINEAR)
# Resize to a smaller size (0.5x scaling)
smaller_image = cv2.resize(image, None, fx=0.5, fy=0.5, interpolation=cv2.INTER_AREA)
# Display images
cv2.imshow("Original Image", image)
cv2.imshow("Bigger Image", bigger_image)
cv2.imshow("Smaller Image", smaller_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT
<img width="950" height="539" alt="image" src="https://github.com/user-attachments/assets/d869264f-c8c2-4bae-9288-6d25352fbfc2" />
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/431e743a-8920-4fe7-b482-4d88ab7778ff" />


