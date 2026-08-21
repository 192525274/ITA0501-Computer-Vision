## PROGRAM
``` PYTHON
import cv2
import numpy as np
image = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
rows, cols, ch = image.shape
pts1 = np.float32([[50, 50], [400, 50], [50, 400], [400, 400]])
pts2 = np.float32([[10, 100], [300, 50], [100, 300], [350, 350]])
matrix = cv2.getPerspectiveTransform(pts1, pts2)
transformed_image = cv2.warpPerspective(image, matrix, (cols, rows))
cv2.imshow("Original Image", image)
cv2.imshow("Perspective Transformed Image", transformed_image)
cv2.imwrite("perspective_transformed.jpg", transformed_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/9e87253e-7306-4399-8d70-873152aa05db" />
<img width="959" height="502" alt="image" src="https://github.com/user-attachments/assets/0689fcd8-f848-4743-95cc-567793034240" />


