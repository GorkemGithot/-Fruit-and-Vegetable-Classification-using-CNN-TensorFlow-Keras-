🍎🥦 Fruit and Vegetable Classification using CNN (TensorFlow & Keras)

This project presents a deep learning-based image classification system built with TensorFlow and Keras, designed to identify 36 different types of fruits and vegetables. The model utilizes a custom CNN architecture and is trained on a labeled dataset using Google Colab and Google Drive for storage and computation.
📁 Dataset Structure

The dataset is organized into three main folders: train, validation, and test. Each subfolder corresponds to a specific fruit or vegetable category.

dataset/
├── train/
│   ├── Apple/
│   ├── Banana/
│   └── ...
├── validation/
│   ├── Apple/
│   ├── Banana/
│   └── ...
└── test/
    ├── Apple/
    ├── Banana/
    └── ...

🚀 Key Features

    ✅ Efficient data loading using image_dataset_from_directory with on-the-fly labeling.

    🌈 Image normalization via Rescaling(1./255) for consistent model input.

    🧱 Custom CNN architecture built with:

        Conv2D layers for spatial feature extraction

        MaxPooling layers for downsampling

        Dropout layers for regularization

        Flatten + Dense layers for classification

    🧠 Optimized with the Adam optimizer and categorical_crossentropy loss for multi-class classification.

    📊 Real-time tracking of training and validation accuracy over 30 epochs.

    🖼️ Visual analysis of model performance using matplotlib plots.

    📦 Model persistence using .h5 format for reusability.

🧠 Training Pipeline Overview

    Input shape: 64x64x3 (RGB images)

    Output: 36-class softmax

    Batch size: 32

    Epochs: 30

    Framework: TensorFlow + Keras

    Platform: Google Colab with Google Drive integration

🧪 Testing Pipeline Overview

    Loads trained .h5 model from Google Drive.

    Preprocesses a test image (resize, scale, batchify).

    Uses .predict() to generate confidence scores.

    Maps output index to human-readable class label.

    Displays the image and prints prediction results.

📊 Output & Evaluation

    ✅ Final validation accuracy printed in console.

    📈 Accuracy curves plotted to visualize learning trends.

    🔍 Test image classification result printed alongside confidence scores.

    🔠 Full list of class names available via test_set.class_names.

📌 Requirements

    Python 3.x

    TensorFlow ≥ 2.x

    NumPy, Matplotlib

    Google Colab or Jupyter Notebook

    (Optional) Git LFS for storing model files over 25 MB
