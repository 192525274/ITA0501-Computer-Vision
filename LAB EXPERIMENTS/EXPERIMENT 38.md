## PROGRAM
```PYTHON
import cv2

def count_faces(image_path):

    # Read image
    image = cv2.imread(image_path)

    # Convert to grayscale
    gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)

    # Load face detector
    face_cascade = cv2.CascadeClassifier(
        cv2.data.haarcascades + "haarcascade_frontalface_default.xml"
    )

    # Detect faces
    faces = face_cascade.detectMultiScale(
        gray,
        scaleFactor=1.1,
        minNeighbors=5
    )

    # Count faces
    face_count = len(faces)

    print("Number of faces detected:", face_count)

    # Draw rectangles
    for (x, y, w, h) in faces:
        cv2.rectangle(
            image,
            (x, y),
            (x + w, y + h),
            (0, 255, 0),
            2
        )

    # Show result
    cv2.imshow("Face Detection", image)

    cv2.waitKey(0)
    cv2.destroyAllWindows()


# Image path
image_path = r"C:\Users\sathw\Downloads\Group photos with friends.jpg"

# Run function
count_faces(image_path)
```
# OUTPUT
<img width="959" height="506" alt="image" src="https://github.com/user-attachments/assets/e0bd8b5b-c781-4ffd-82d3-604c7a19118a" />
<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/59ad605f-b531-468f-aca4-d70b97292dab" />


