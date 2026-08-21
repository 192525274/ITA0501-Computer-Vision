## PROGRAM
``` PYTON
import cv2
image = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
flipped_image = cv2.flip(image, 1)
rotated_image = cv2.rotate(flipped_image, cv2.ROTATE_180)
cv2.imshow("Original Image", image)
cv2.imshow("Rotated 180-degree Clockwise Along Y-axis", rotated_image)
cv2.imwrite("rotated_image.jpg", rotated_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/1cfba3ba-4219-4682-b070-b697819ac8a7" />
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/bb3df08a-31e8-4a2a-86b8-9d53725c3af2" />


