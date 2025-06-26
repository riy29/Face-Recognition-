# Face Recognition using PCA + ANN

This project implements a web-based face recognition system using Principal Component Analysis (PCA) for feature extraction and Artificial Neural Networks (ANN) for classification. The system is designed to recognize faces from a dataset of images and predict identities with high accuracy.

## Models Used
- PCA (Scikit-learn)
- ANN (TensorFlow / Keras)
- Uses Numpy and Scipy

## Workflow
1. Upload & extract dataset
2. Convert images to grayscale & resize to 100x100
3. Flatten & scale using `StandardScaler`
4. Apply PCA for dimensionality reduction
5. Train an ANN model
6. Save the model, PCA, scaler, and labels
7. Use trained model to predict new face images

## How to Run

### Backend (Flask)
1. **Set up your environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`

### Install dependencies:

 1. pip install flask numpy opencv-python scikit-learn tensorflow joblib flask-cors

### Run the backend:

1. cd backend
2. python app.py

### Frontend
Open frontend/index.html in your web browser.

### API Routes
/upload [POST]

Accepts a .zip file with the following structure:

dataset.zip
├── person1/
│   ├── img1.jpg
│   └── img2.jpg
├── person2/
│   ├── img1.jpg
│   └── img2.jpg






