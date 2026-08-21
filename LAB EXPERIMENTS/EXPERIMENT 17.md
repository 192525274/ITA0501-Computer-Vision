## PROGRAM
``` PYTHON
import cv2
import numpy as np
# Read the input image
image = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
# Convert the image to grayscale
gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
# Apply Sobel filter in X and Y directions
sobel_x = cv2.Sobel(gray, cv2.CV_64F, 1, 0, ksize=3) # Gradient in X direction
sobel_y = cv2.Sobel(gray, cv2.CV_64F, 0, 1, ksize=3) # Gradient in Y direction
# Convert gradients to absolute scale
sobel_x = cv2.convertScaleAbs(sobel_x)
sobel_y = cv2.convertScaleAbs(sobel_y)
# Combine the gradients
sobel_combined = cv2.addWeighted(sobel_x, 0.5, sobel_y, 0.5, 0)
# Display images
cv2.imshow("Original Image", image)
cv2.imshow("Sobel X", sobel_x)
cv2.imshow("Sobel Y", sobel_y)
cv2.imshow("Sobel Combined", sobel_combined)
# Save the results
cv2.imwrite("sobel_x.jpg", sobel_x)
cv2.imwrite("sobel_y.jpg", sobel_y)
cv2.imwrite("sobel_combined.jpg", sobel_combined)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT
<img width="959" height="501" alt="image" src="https://github.com/user-attachments/assets/2fd70c9c-57c9-4c80-be15-67097e70f5cc" />
<img width="959" height="502" alt="image" src="https://github.com/user-attachments/assets/d600b72b-8f08-4c34-be16-4f1980842907" />
<img width="959" height="504" alt="image" src="https://github.com/user-attachments/assets/d375be52-bde8-4263-a8b6-da0a25c0547a" />
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/0132cec6-a29c-4da7-813b-51c86aee53d8" />




