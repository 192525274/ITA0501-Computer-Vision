## PROGRAM
```Python
import cv2
image = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
edges = cv2.Canny(gray_image, 100, 200)
cv2.imshow("Original Image", image)
cv2.imshow("Edge Detected Image", edges)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT
<img width="959" height="505" alt="image" src="https://github.com/user-attachments/assets/08f8e8a4-5351-4bbb-9726-04f09ef61c5f" />
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/ae8c6323-fe99-4c26-a294-bacfdd7b3bf3" />


