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

### Project Timeline:
#### Edward:
#### Anton:
