## Condition-Aware Dereverberation using a 2D CNN

This repository contains a deep learning project for **dereverberation**, the process of removing echo from audio signals. The model is a custom-built 2D Convolutional Neural Network (CNN) that learns to transform noisy, reverberant audio into a clean, clear signal.

A key feature of this project is its use of **conditional training**. The model is not only trained on spectrograms but is also conditioned on the **Mean T60** value, a scientific measure of reverberation time. This allows the model to become "acoustically aware," enabling it to more effectively handle varying levels of echo.

### Key Features
* **Custom 2D CNN Architecture**: A tailored neural network designed for end-to-end dereverberation.
* **Condition-Aware Training**: The model uses `T60` metadata to guide the training process, leading to improved performance.
* **Spectrogram-Based Processing**: Audio is converted into a visual spectrogram representation, allowing the 2D CNN to treat the task as an image-to-image translation problem.
* **Structured Data Pipeline**: A clean and efficient Python script for loading and preparing audio data from a CSV metadata file.

### Technologies
* **PyTorch**: The deep learning framework used for building and training the model.
* **NumPy**: For numerical operations and data handling.
* **pandas**: For loading and managing the audio metadata from the CSV file.
* **SciPy / Matplotlib**: For signal processing and data visualization.
