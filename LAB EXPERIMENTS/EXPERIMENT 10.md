## PROGRAM
```PYTHON
import cv2
img = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
rotated_img = cv2.rotate(img, cv2.ROTATE_90_CLOCKWISE)
cv2.imshow("Rotated Image", rotated_img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT 
<img width="553" height="503" alt="image" src="https://github.com/user-attachments/assets/3dec16bb-8308-472e-ba6a-008db35ab518" />


