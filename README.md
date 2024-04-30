# Neural Network-Based Image Recognition Using CNN



## Model Architecture and Parameters

The input layer takes a 224x224 pixel image in RBG format (3 colour inputs). The output layer has 15 classes as there are 15 birds categories to predict.
The layers that we used are:

- Conv2D

   - A convolutional layer for two-dimensional inputs.
   - Applies filters to an image to help outline key features of the image.
   - The important layer in convolutional neural networks and computer vision.

- MaxPool2D

   - Summarises the features in a feature map (which is generated by the convolutional layer).
   - Therefore reduces the amount of work for the neural network.

- Dense

    - A layer where all the neurons in the previous layer are connected to all the neurons in the 'dense' layer.
    - It is used to classify images based on the outputs of convolutional layers.

- Flatten

    - Flattens the input into a one dimension.
    - Used so that the input can be fed into a next neuron.

- Activation functions

    - Add a non linearity to the network, allowing the predictions to better fit the results.
    - Improves accuracy.

- To overcome over fitting 

    - Data augmentation: generates additional data from current train dataset and applies some rotation/zooming to help the model have a better performance.

    - Dropouts: remove a percentage of the outputs of the last layer. In our case, we are removing 50 percent of outputs of the second hidden layer each iteration which leads to reduce the over fitting.

- 40 epochs  and a batch size of 10 (model updates after each 10 samples) were used. 

## Results

Best Results from CNN

- Training Set --> 86.90 %
- Test Set  --> 82. 67 % 
- Validation Set  --> 82.67 %

## Further Ideas
The model had a decent performance on the test dataset. Our future goal is to figure out how to increase the model’s accuracy by either tuning the hyperparameters to better find a well-suited arrangement of the layers or implementing a pretrained model .

## Bird Species Dataset

Data set of 450 bird species. 70,626 training images, 22500 test images(5 images per species) and 2250 validation images(5 images per species.  All images are 224 X 224 X 3 color images in jpg format. Data set includes a train set, test set and validation set. Each set contains 450 sub directories, one for each bird species. 

The dataset is available on Kaggle. You can find more information and download the data [here](https://www.kaggle.com/datasets/gpiosenka/100-bird-species?resource=download)

## Credits
[Lucas Hawranke](https://github.com/lucashawranke), [Mahmoud El Hazzouri](https://github.com/melhazzouri), [Mahyar Fazelzade](https://github.com/Mahyar-Fazelzadeh)
