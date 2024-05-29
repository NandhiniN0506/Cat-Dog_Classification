**SVM Classification for Cats and Dogs using Data Augmentation**

**Overview**

This project demonstrates the use of a Support Vector Machine (SVM) classifier to distinguish between images of cats and dogs. To enhance model performance and mitigate overfitting, data augmentation is utilized.

**Prerequisites**

            * Python 3.x
            * TensorFlow
            * OpenCV
            * scikit-learn
            * matplotlib
            * numpy

**Dataset**
The "Cats and Dogs" dataset from TensorFlow is used. It is automatically downloaded and extracted by the script.

**Data Augmentation**

Data augmentation increases the diversity of the training set by applying random transformations to the images, such as:

                                                * Rescaling
                                                * Horizontal flipping
                                                * Rotation
                                                * Zooming
This ensures the model encounters varied representations of the images, aiding in better generalization.

**Workflow**

**1. Data Loading and Preprocessing**

The dataset is downloaded and organized into training and validation directories.

**2. Data Augmentation**

Using ImageDataGenerator, various transformations are applied to the training images. This process helps in artificially increasing the size and variability of the training dataset.

**3. Feature Extraction**

Images are flattened and standardized to be used as input features for the SVM model.

**4. Model Training**

The SVM classifier is trained on the augmented dataset.

**5. Evaluation**

The model's accuracy is evaluated using the validation dataset. A function is also provided to predict and display the class of a single image, showing whether it is a cat or a dog.

**6. Prediction and Display**

A utility function is included to predict the class of a single test image and display the image along with the prediction label.

**Conclusion**

Using data augmentation and SVM, the project effectively classifies images of cats and dogs, demonstrating a robust method to handle small datasets and improve model generalization.
