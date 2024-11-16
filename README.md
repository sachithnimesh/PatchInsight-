
# **PatchInsight**

**PatchInsight** is a deep learning-based application designed to classify clothing images into two categories: **patched** and **non-patched**. This project leverages transfer learning with **InceptionV3** to achieve highly accurate predictions and provides an interactive interface for users to upload images and receive real-time results.

---

## **Features**

- Classifies images into **patched** or **non-patched** categories.
- Fine-tuned **InceptionV3** model for high accuracy.
- Web-based interface for easy image uploads and predictions.
- Fully implemented in **Python**, using **TensorFlow** and **Flask**.

---

## **Demo**

Upload an image of clothing, and the application will predict whether it contains a patch.

![Demo](link_to_demo_image_or_gif)

---

## **Getting Started**

Follow these steps to set up and run the project locally or in Google Colab.

### **Prerequisites**

Make sure you have the following installed:
- Python 3.8 or later
- TensorFlow
- Flask
- Pillow

Install the required Python packages:
```bash
pip install tensorflow flask pillow flask-ngrok
```

---

### **Project Structure**

```
PatchInsight/
├── dataset/                   # Folder for training and validation data
├── inceptionv3_best_model.h5  # Pre-trained model
├── app.py                     # Flask application script
└── README.md                  # Project documentation
```

---

## **Usage**

### **Step 1: Clone the Repository**
```bash
git clone https://github.com/yourusername/PatchInsight.git
cd PatchInsight
```

### **Step 2: Run the Application**

1. **Place the Model**:
   Ensure `inceptionv3_best_model.h5` is in the project directory.

2. **Run the Flask App**:
   ```bash
   python app.py
   ```

3. **Access the App**:
   - If running locally, open your browser and go to `http://127.0.0.1:5000`.
   - If running on Google Colab, you’ll get an **ngrok** link to access the app.

---

## **Model Details**

- **Model**: InceptionV3
- **Training**:
  - Dataset: Clothing images categorized as patched and non-patched.
  - Image Preprocessing: Resized to 360x640 px, normalized to [0, 1].
  - Fine-Tuning: Last 15 layers of InceptionV3 unfrozen.
  - Optimized using learning rate scheduling and dropout regularization.
- **Validation Accuracy**: 100%

---

## **How It Works**

1. Users upload an image through the web interface.
2. The image is preprocessed to match the model's input size.
3. The trained model predicts the class (patched or non-patched).
4. Results (class and confidence) are displayed.

---

## **Sample Prediction**

```bash
Uploaded Image: test_image.jpg
Prediction: Patched
Confidence: 98.7%
```

---

## **Future Enhancements**

- Expand dataset for greater generalization.
- Add multi-class classification for detecting different types of patches.
- Deploy to cloud platforms like AWS or Google Cloud for wider accessibility.

---

## **Contributing**

Contributions are welcome! If you have ideas for improvement, feel free to:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Submit a pull request.

---
