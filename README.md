# Udacity_image_classifier
 In this project, code developed for an image classifier built with PyTorch, then converted into a command line applications: train.py, predict.py.

The image classifier to recognize different species of flowers. Dataset contains 102 flower categories.

In Image Classifier Project.ipynb Alexnet from torchvision.models pretrained models was used. It was loaded as a pre-trained network, based on which defined a new, untrained feed-forward network as a classifier, using ReLU activations and dropout. Trained the classifier layers using backpropagation using the pre-trained network to get the features. The loss and accuracy on the validation set were tracked to determine the best hyperparameters.

Command line applications train.py and predict.py
For command line applications there is an option to select either Alexnet or VGG13 models.

Following arguments mandatory or optional for train.py

'data_dir'. 'Provide data directory. Mandatory argument', type = str
'--save_dir'. 'Provide saving directory. Optional argument', type = str
'--arch'. 'Vgg13 can be used if this argument specified, otherwise Alexnet will be used', type = str
'--lrn'. 'Learning rate, default value 0.001', type = float
'--hidden_units'. 'Hidden units in Classifier. Default value is 2048', type = int
'--epochs'. 'Number of epochs', type = int
'--GPU'. "Option to use GPU", type = str
Following arguments mandatory or optional for predict.py

'image_dir'. 'Provide path to image. Mandatory argument', type = str
'load_dir'. 'Provide path to checkpoint. Mandatory argument', type = str
'--top_k'. 'Top K most likely classes. Optional', type = int
'--category_names'. 'Mapping of categories to real names. JSON file name to be provided. Optional', type = str
'--GPU'. "Option to use GPU. Optional", type = str
