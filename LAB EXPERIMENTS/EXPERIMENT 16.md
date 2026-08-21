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
<img width="959" height="505" alt="image" src="https://github.com/user-attachments/assets/4247c08e-cca8-40e8-839b-75e0bdf76c18" />
<img width="959" height="498" alt="image" src="https://github.com/user-attachments/assets/3e3e3869-fcfc-409f-8072-5c6fb4323636" />
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/fa6daf21-9834-4e09-a17a-447b9e322ce9" />
<img width="959" height="502" alt="image" src="https://github.com/user-attachments/assets/de8f8057-6cf8-4c2b-b0ad-c19f6ff47890" />




