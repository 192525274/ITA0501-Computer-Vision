##PROGRAM
``` PYTHON
import cv2
import numpy as np
image = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
rows, cols, ch = image.shape
pts1 = np.float32([[50, 50], [200, 50], [50, 200]])
pts2 = np.float32([[10, 100], [200, 50], [100, 250]])
matrix = cv2.getAffineTransform(pts1, pts2)
transformed_image = cv2.warpAffine(image, matrix, (cols, rows))
cv2.imshow("Original Image", image)
cv2.imshow("Affine Transformed Image", transformed_image)
cv2.imwrite("affine_transformed.jpg", transformed_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/51e3ad8b-ef9a-49b6-94aa-b5842d2ff0cb" />
<img width="959" height="502" alt="image" src="https://github.com/user-attachments/assets/3f669eed-4e25-406c-97b2-87ff155ef7a2" />


