# Emotion Classification from Facial Expressions

## Task Description

The objective of this project is to categorize each face based on the emotion shown in the facial expression into one of seven categories:

- 0 = Angry
- 1 = Disgust
- 2 = Fear
- 3 = Happy
- 4 = Sad
- 5 = Surprise
- 6 = Neutral

## Dataset

The dataset used for this task consists of 48x48 pixel grayscale images of faces. The faces have been automatically centered and scaled so that each face occupies a similar amount of space within the image. Note that the dataset is imbalanced, which poses a challenge for training accurate models.

## Models

### Model 1: CNN with Data Augmentation

- **Architecture:** Convolutional Neural Network (CNN)
- **Training:** Trained for 10 epochs with data augmentation techniques to improve generalization.
- **Performance:**
  - Train Accuracy: 36.96%
  - Validation Accuracy: 37.27%
  - Overall F1 Score: 0.21
  - Notably performed poorly in classifying images labeled as 'Disgust'.

### Model 2: Transfer Learning with ResNet50

- **Architecture:** Transfer learning using a pre-trained ResNet50 model.
- **Training:** Trained for 10 epochs with class weights to address the issue of imbalanced data.
- **Performance:**
  - Train Accuracy: 67.28%
  - Validation Accuracy: 64.80%
  - Overall F1 Score: 0.65

## Conclusion

Two models were trained to classify facial expressions into seven emotion categories. The CNN with data augmentation showed limited success, particularly struggling with the 'Disgust' category. In contrast, the transfer learning approach using ResNet50 with class weights yielded significantly better performance, achieving a higher overall F1 score.

## Future Work

Future improvements could include:
- Further tuning of hyperparameters.
- Experimenting with different architectures and transfer learning models.
- Applying advanced techniques to handle class imbalance more effectively.
- Increasing the number of training epochs.


