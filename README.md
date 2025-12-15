# Digit_Recognition
Developed a real-time handwritten digit recognition system using CNNs trained on MNIST and custom webcam data, achieving robust digit classification using OpenCV and TensorFlow.

🚀 Features
📸 Webcam-based custom digit dataset collection
🧠 CNN trained on MNIST + custom handwritten digits
🔄 Data augmentation for better generalization
🎥 Real-time digit recognition using OpenCV
📦 Model saving and reloading
🖐️ ROI-based digit detection
🔢 Supports digits 0–9
🛠️ Tech Stack
Python
TensorFlow / Keras
OpenCV
NumPy
MNIST Dataset

📁 Project Structure
digit-recognition/
│
├── dataset/
│   ├── 0/
│   ├── 1/
│   ├── ...
│   └── 9/
│
├── collect_digits.py
├── train_mnist_custom.py
├── train_custom_only.py
├── realtime_prediction.py
├── digit_recognition_model.h5
├── custom_digit_model.h5
├── requirements.txt
└── README.md

🧠 Step 2: Model Training
Training Data
MNIST Dataset
Custom webcam digit images
Combined to improve real-world accuracy
Data Augmentation
Rotation
Zoom
Width & height shift
Shear
Brightness variation

CNN Architecture
Conv2D (32) → Conv2D (32) → MaxPool → Dropout
Conv2D (64) → Conv2D (64) → MaxPool → Dropout
Flatten
Dense (256)
Dropout
Dense (10 - Softmax)
Training Configuration
Optimizer: Adam
Loss: Categorical Crossentropy
Epochs: 10
Image size: 28×28
Output classes: 0–9

🎥 Step 3: Real-Time Digit Recognition
Live webcam feed
Digit drawn inside ROI
Image preprocessing:
Grayscale
Thresholding
Normalization
Model predicts digit instantly
Press q to exit.

🔮 Future Enhancements
📊 Confidence score display
✏️ Digit drawing canvas (instead of webcam)
📱 Mobile / edge deployment
🧠 Transfer learning (LeNet / MobileNet)
📈 Accuracy & loss visualization
🧪 Digit segmentation for multiple digits
