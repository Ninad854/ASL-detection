# ASL-detection
# Hand Gesture Recognition Project

This project captures hand gesture images, processes them, trains a model, and performs real-time recognition using MediaPipe and OpenCV.

---

## 📁 Scripts Overview

### 1. Image Data Collection (`collect_data.py`)

- Captures images from the webcam.
- Saves 26 classes (A-Z) with 100 images each.
- Organizes images into class-specific folders in `./data`.

### 2. Dataset Creation (`create_dataset.py`)

- Processes images using [MediaPipe Hands](https://google.github.io/mediapipe/solutions/hands.html).
- Extracts normalized hand landmark coordinates.
- Saves feature vectors and labels to `data.pickle` for training.

### 3. Model Training (`train_model.py`)

- Loads dataset from `data.pickle`.
- Trains a Random Forest classifier to recognize gestures.
- Evaluates accuracy and saves the model as `model.p`.

### 4. Real-time Gesture Recognition (`run_model.py`)

- Uses webcam feed to detect hand gestures live.
- Applies the trained model to predict and display gestures on screen.

---

## 🚀 How to Use

1. **Collect Data:**  
   Run `collect_data.py` to capture your gesture images.

2. **Create Dataset:**  
   Run `create_dataset.py` to extract features.

3. **Train Model:**  
   Run `train_model.py` to train and save the model.

4. **Run Recognition:**  
   Run `run_model.py` to test real-time gesture recognition.

---


---

## 📬 Contact

Feel free to reach out if you have any questions or suggestions!

---

**Happy Coding!** 🎉
