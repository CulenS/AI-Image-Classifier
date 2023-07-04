# AI-Image-Classifier


The project aims to classify images into "Fake" and "Real" categories using the VGG16 model and transfer learning on the CIFAKE Dataset. The steps followed in the project can be summarized as follows:

1) Dataset Preparation: The project utilized a dataset containing images of both real and fake images. The dataset was split into training and testing sets.For convenience I have trained on 4000 images and tested on 400 images.
2) Model Architecture: The VGG16 model, pre-trained on the ImageNet dataset, was used as the base model. The last few layers were modified to suit the binary classification task. A fully connected layer with a sigmoid activation function was added as the output layer.
3) Model Training: The model was compiled with appropriate loss and optimization functions. Data augmentation techniques such as rescaling, shearing, zooming, and horizontal flipping were applied to the training data to improve model generalization. The model was trained on the augmented training data.
4) Model Evaluation: The trained model was evaluated on the testing data. Predictions were made on the test set, and performance metrics such as accuracy, confusion matrix, classification report, and mean average precision (mAP) were calculated to assess the model's performance.
5) Visualization: Various visualizations were created to understand the model's predictions better. These included a confusion matrix, loss plot, precision-recall curve, and F1 curve. Additionally, a sample of test images was selected randomly to display the predicted labels and class probabilities.
