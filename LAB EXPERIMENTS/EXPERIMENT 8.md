## PROGRAM
``` PYTHON
import cv2
image = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
cv2.imshow("Original Image", image)
cv2.imshow("Grayscale Image", gray_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/6df79150-618a-482c-99ee-71fbdbc80d12" />
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/a4b4ab0c-0868-46aa-a140-f81d269dab89" />


