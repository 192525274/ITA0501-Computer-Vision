## PROGRAM
```PYTHON
import cv2
import numpy as np
import matplotlib.pyplot as plt
def analyze_histogram(image_path):
    image = cv2.imread(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
    if image is None:
        print("Error: Unable to load image.")
        return
    color_channels = ('b', 'g', 'r')
    plt.figure(figsize=(10, 5))
    for i, color in enumerate(color_channels):
        histogram = cv2.calcHist([image], [i], None, [256], [0, 256])
        plt.plot(histogram, color=color, label=f"{color.upper()} Channel")
    plt.xlim([0, 256])
    plt.title("Color Histogram Analysis")
    plt.xlabel("Pixel Intensity")
    plt.ylabel("Frequency")
    plt.legend()
    plt.show()
analyze_histogram(r"C:\Users\sathw\OneDrive\Desktop\Computer Vision\Sample image.jpeg")
```
# OUTPUT
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/51978366-6ec1-4a6b-9218-e238df5b992a" />

