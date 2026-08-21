## PROGRAM
``` Python
import cv2
image = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
blurred_image = cv2.GaussianBlur(image, (15, 15), 0) 
cv2.imshow("Original Image", image)
cv2.imshow("Blurred Image", blurred_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/42e5fcb3-2abd-4fba-9173-ebc0bfba4075" />
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/f3d296c4-2beb-47a7-a01c-79f3e2fa9429" />


