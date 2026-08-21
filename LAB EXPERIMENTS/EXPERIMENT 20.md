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
# Wait for a key press and close all windows
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT
<img width="959" height="502" alt="image" src="https://github.com/user-attachments/assets/3b5cc66c-fae7-413e-94d0-2f47406559ee" />
<img width="959" height="502" alt="image" src="https://github.com/user-attachments/assets/377c6b88-6817-4481-9154-52ad8a274faf" />
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/7d82df90-8d27-4c5f-9b93-82f83be249ea" />
<img width="959" height="502" alt="image" src="https://github.com/user-attachments/assets/7dfb9bc0-6d3b-4aa0-96d0-285b01436f66" />



