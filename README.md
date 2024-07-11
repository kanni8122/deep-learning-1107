This project focuses on predicting the coordinates (x, y) of a pixel with a value of 255 in a 50x50 grayscale image using deep learning techniques. 
Each image in the dataset contains a single pixel set to 255, while all other pixels are 0. The location of the pixel with a value of 255 is randomly assigned, and the task is to accurately predict its coordinates. 
The project involves generating a synthetic dataset, building a convolutional neural network (CNN) model, training the model, and evaluating its performance.

The dataset is generated using a custom function that creates 50x50 pixel grayscale images. Each image has one pixel with a value of 255 and all other pixels set to 0. 
The coordinates of the pixel with a value of 255 serve as the target labels for training. The dataset is split into a training set with 8000 samples and a validation set with 2000 samples to ensure sufficient data for model training and evaluation.

The model architecture is a simple convolutional neural network (CNN) designed to capture the spatial features of the images. 
It consists of three convolutional layers with increasing filter sizes, followed by a flatten layer to convert the 2D feature maps to a 1D vector. This is followed by two dense layers, with the final layer outputting the coordinates (x, y). 
The model is trained using the Adam optimizer with a learning rate of 0.001 and mean squared error (MSE) as the loss function. The training process involves running the model for 10 epochs.

To evaluate the model's performance, the ground truth and predicted coordinates are visualized for a sample of validation images. 
This helps in understanding how well the model can predict the location of the pixel with a value of 255. 
The results and visualizations provide insights into the model's accuracy and areas for potential improvement.

To run this project, ensure you have the necessary dependencies installed: TensorFlow, NumPy, and Matplotlib. You can install these dependencies using the provided requirements.txt file. The complete implementation, including dataset generation, model training, and evaluation, is available in the provided Jupyter notebook. This project demonstrates the application of deep learning techniques to a specific regression problem, focusing on the approach and implementation rather than achieving the highest possible accuracy.
