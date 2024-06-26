# Image Data Classification using Random Forest Classifier (Sklearn)

## Aim
The goal of this project is to classify images of cats and dogs using a Random Forest Classifier from the Scikit-learn library. We aim to explore how machine learning models can be applied to image classification tasks.

## Dataset
This dataset consists of images categorized into two classes: Cats and Dogs. It is suitable for binary classification in computer vision tasks.

### Dataset Source
The dataset is sourced from Kaggle:
- [Microsoft Cats vs Dogs Dataset](https://www.kaggle.com/datasets/shaunthesheep/microsoft-catsvsdogs-dataset)

## Installation
To run this project, install the required dependencies using the following command:

```bash
pip install numpy==1.22.3 pandas matplotlib scikit-image scikit-learn joblib opencv-python imageio[pyav]
```

## Usage
1. **Import Necessary Libraries**: Import all required libraries and suppress warnings.
2. **Load, Resize & Store Images**: Resize images from the 'PetImages' folder, categorizing them into 'Dog' and 'Cat', and store them in a serialized format (.pkl).
3. **Read and Preprocess Data**: Load the resized images, preprocess them (normalize), and split them into training and testing sets.
4. **Feature Extraction using HOG**: Extract features using Histogram of Oriented Gradients (HOG) from the images.
5. **Hyperparameter Tuning**: Tune the Random Forest Classifier's hyperparameters using RandomizedSearchCV to optimize model performance.
6. **Fit and Predict**: Train the final model with the optimized parameters and predict on the test set.
7. **Custom Prediction Function**: Define a function to predict labels for custom images using the trained model.

## Files Included
- `README.md`: This file, providing an overview of the project.
- `main.ipynb`: Jupyter notebook containing the entire code with explanations and steps.
- `PetImages/`: Folder containing original images of cats and dogs.

## References
- [Scikit-learn Documentation](https://scikit-learn.org/stable/documentation.html)
- [Kaggle Cats vs Dogs Dataset](https://www.kaggle.com/datasets/shaunthesheep/microsoft-catsvsdogs-dataset)

