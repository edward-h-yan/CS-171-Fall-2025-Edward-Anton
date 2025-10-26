# CS-171-Fall-2025-Edward-Anton

### Authors: Edward Yan, Anton Clayton

### Description:
The question we want to answer during this project is whether a machine learning model has an easier time classifying images if they are distinct from each other, or if the model would have similar success on similar images. We will train one model to recognize different butterfly species and one model to recognize different animals. Our initial hypothesis is that the model trained to recognize different animals would be much more successful, as there would be less overlap between the shape and coloration of the animals and environment. This is how we, as humans, see this problem of pattern recognition. However, as we have seen in class, a red crab can look very similar to a light blue squid to a machine.

## Project Outline/Plan:
### Data Collection Plan:
#### Edward:
#### Anton:
I will be using the Animals-10 image dataset from Kaggle for this image classification task. This dataset contains images across ten distinct categories: dog, cat, horse, spider, butterfly, chicken, sheep, cow, squirrel, and elephant. The images are already organized into separate subdirectories, with each directory's name corresponding to its respective animal class. To create robust training and testing datasets for the model, I will use a stratified split to ensure that the class distribution within the resulting train and test sets is proportional to the original dataset. This way, there will not be class imbalance issues during evaluation. Furthermore, I will apply data augmentation techniques, such as random rotations, shifts, flips, and zooms, to the Training Dataset. By doing this, I will artificially increase the size and diversity of my training data, which will, in turn, help improve the model's generalization capability and reduce the risk of overfitting. I will ensure the Testing dataset remains completely unaltered to guarantee a fair evaluation of the final model on the original images.

### Model Plans:
#### Edward:
#### Anton:
I will utilize a Convolutional Neural Network (CNN) for this 10-class image classification task. As we have learned in class, CNNs are specifically designed to process image data by automatically and adaptively learning spatial hierarchies of features through convolutional layers so it will be the best choice for this task. For this CNN's framework, I will implement multiple convolution layers (followed by ReLU), pooling, batch normalization, and a final set of fully connected layers. The final output layer will have 10 neurons (one for each animal class). For the training process, I plan to use Cross-Entropy Loss for the loss function and for the Optimizer, I will use the Adam Optimizer. Until I test out what works best for the model, other parameters such as number of epochs and learning rate are undecided for now.

### Project Timeline:
#### Week 11
- Digest dataset and work on reading in and separating image data
#### Week 12
- Create training and testing datasets. Use data augmentation techniques for the training set.
#### Week 13
- Create basic working CNN model with plots to show losses and performance
#### Week 14
- Optimize model's parameters and test model on various parameters. Add techniques to combat overfitting and adjust model's layers as needed.
#### Week 15
- Final touches to model and create presentation for Week 16
#### Week 16
- Presentation in class
