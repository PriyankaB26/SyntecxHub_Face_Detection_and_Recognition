# SyntecxHub_Face_Detection_and_Recognition

## 📌 Project Overview

This project implements a **Face Detection and Face Recognition system** using **OpenCV** and **deep face embeddings**. 
The system can:

* Detect faces in images
* Recognize **known individuals** from a trained dataset
* Handle **multiple faces** in a single image
* Draw **bounding boxes and labels** only for recognized faces
* Easily **add new people** without changing code

The project is implemented and tested in **Google Colab**, and can be extended to video or webcam-based recognition.

---

## 🧠 Technologies & Libraries Used

* **Python 3**
* **OpenCV (cv2)** – image processing & drawing bounding boxes
* **face_recognition** – face detection and 128-D face embeddings (built on dlib)
* **NumPy** – numerical operations
* **Pickle** – saving and loading face encodings

## 🔹 Face Registration (Training Phase)

This project **does not train a neural network from scratch**. Instead, it:

1. Detects faces in images
2. Converts each face into a **128-dimensional embedding** using a pre-trained deep learning model
3. Stores these embeddings along with labels (person names)


📌 **Labels are automatically taken from folder names**

---

## 🔹 How to Add New People 

To add a new person **NO CODE CHANGES ARE REQUIRED**.

### Steps:

1. Create a new folder inside `data/known_faces/`
2. Name the folder with the person’s name (this becomes the label)
3. Add 5–20 clear face images of that person
4. Re-run the face registration script

Example:

```
data/known_faces/Alia_Bhatt/
├── img1.jpg
├── img2.jpg
```

✔ Folder name → label
✔ Images → training data



##  Output

![Face Recognition Output](output1.png)

