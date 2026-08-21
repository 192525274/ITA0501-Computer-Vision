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
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/98f98023-b2f0-47ee-860c-dd431374a082" />
<img width="959" height="504" alt="image" src="https://github.com/user-attachments/assets/31802e09-1ef5-4c86-b1cf-47588d354d26" />

