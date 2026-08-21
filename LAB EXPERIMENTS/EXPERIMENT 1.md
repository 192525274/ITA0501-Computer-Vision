## PROGRAM
```Python
import cv2
image = cv2.imread(r"C:\Users\sathw\OneDrive\Pictures\Screenshots\Screenshot 2026-07-16 105735.png")
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
cv2.imshow("Original Image", image)
cv2.imshow("Grayscale Image", gray_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/ccbf7d78-e07f-4adc-80ab-a71c7d4d5a64" />
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/42e17578-6324-402a-b720-04ffb38cb258" />

