
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

![Demo](data:image/jpeg;base64,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)

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
