CNN Image Classification with MNIST
This project applies a convolutional neural network (CNN) to the MNIST dataset of handwritten digits. The goal is to train a deep learning model that can accurately classify digits (0–9) from grayscale images.
Dataset
•	MNIST dataset: 60,000 training images, 10,000 test images
•	Each image: 28x28 pixels, grayscale
Methods
•	Data reshaping and normalization
•	One-hot encoding of labels
•	CNN architecture with convolutional, pooling, and dense layers
•	Model training and evaluation with Keras/TensorFlow
•	Confusion matrix used to check classification accuracy
Results
The CNN achieved high accuracy on the test set, correctly classifying the majority of digits. The confusion matrix showed strong overall performance, with occasional misclassifications on similar-looking digits (e.g., 4 and 9).
Tools
•	Python (TensorFlow/Keras, NumPy, Matplotlib)
•	Jupyter Notebook
Future Work
•	Experiment with deeper CNNs or regularization techniques
•	Apply data augmentation to improve generalization
•	Extend the model to other image datasets beyond MNIST
