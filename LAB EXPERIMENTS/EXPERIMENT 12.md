## PROGRAM
``` PYTHON
import cv2
image = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
flipped_image = cv2.flip(image, 1)
rotated_image = cv2.rotate(flipped_image, cv2.ROTATE_90_COUNTERCLOCKWISE)
cv2.imshow("Original Image", image)
cv2.imshow("Rotated 270-degree Clockwise Along Y-axis", rotated_image)
cv2.imwrite("rotated_image_270.jpg", rotated_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/f8fcada9-c3e0-41ca-bc7a-4eafe0096ba8" />
<img width="553" height="503" alt="image" src="https://github.com/user-attachments/assets/ab682e9a-400d-4d92-87cd-7fae47402034" />


