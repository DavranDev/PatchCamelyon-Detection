# PCam-CNNs-Attention-Analysis

## Overview 
This project explores the use of Convolutional Neural Networks (CNNs) enhanced with attention mechanisms to improve the classification of metastatic tissue in histopathological images from the PatchCamelyon (PCam) dataset. The dataset consists of 327,680 labeled images from lymph node sections, which serve as a benchmark for automated cancer detection. By integrating attention layers (channel and spatial attention) into the CNN architecture, the model can focus on the most critical regions in the images, improving classification accuracy and interpretability. The results show that the CNN with attention outperforms the baseline model, achieving higher accuracy (83.1% vs. 78.6%), F1 score (80.8% vs. 73.6%), and recall (70.9% vs. 59.8%), while reducing false negatives and improving generalization. This work demonstrates the effectiveness of attention mechanisms for enhancing CNN models in complex tasks like medical imaging, with potential applications in automated cancer detection. 

## Files 

#### a) demo.py
This contains the data loading, data prepreocessing/augmentation, EDA, selected model run, and model evaluation. No training is required to run this file. It directly imports the trained model. (Also can be accessed through google colab at https://drive.google.com/file/d/1JRnXmQPl0BxD_LNqfIU3ELETqymIN-DB/view?usp=drive_link)

#### b) CNN_GridSearch.ipnyb
This contains code and method for getting best hyperparameters and parameters for our baseline CNN model. (Also can be accessed through google colab at https://drive.google.com/file/d/18Pjgwk8lPHcY4y7qs9PzvvPLEw5pgBjS/view?usp=drive_link)

#### c) CNN_extended_epochs.ipnyb 
This contains training and evaluation for the CNN with complete training set. (Also can be accessed through google colab at https://drive.google.com/file/d/1NfYhlRzimA08ka4PO7PvhRCz7D_PMjPn/view?usp=drive_link )

#### d) Improved_CNN+Attention_layer_dataug_reg.ipnyb 
This contains the training and evaluation for the selected model which includes CNN + Attention Architecture. (Also can be accessed through google colab at https://colab.research.google.com/drive/1gVk4dPkoGV3rCNqehqwLBhpHK9wkCLSo)

#### e) final_model_attention_improved.h5
This file contains the pre-trained weights for the improved CNN model with attention mechanisms. To use these weights for training, load the .h5 file into your model using TensorFlow/Keras. (Also can be accessed through google colab at https://drive.google.com/file/d/1mj7Ejm9vELGmrUhXYd8cT-p3Y2kHHZm6/view?usp=drive_link)

## How to Run?
1. For ".ipnyb" files ( using Google Colab/Jupyter) - For google colab, Please use above corresponding links and paste in your Google Chrome browser. Navigate to the first cell, In the "Runtime" option in the menu bar, select "Run All". Similar steps to be followed for Jupyter.
2. For ".py" file - Python needs to be installed on your local system. Please use either command line or any code editor to run the ".py" file
3. For using ".h5" file for training - Load the weights into your model by adding the following line in your script or notebook: model.load_weights("final_model_attention_improved.h5"). Please make sure that the downloaded weights are in the same folder as the demo.py OR the alterntative to run the demo.py is directly running the demo file from the colab link provided above.
    
## Requirements 
Infrastructure supporting:
1. ".ipnyb" files i.e. either Google Colab or Jupyter
2. ".py" files.


