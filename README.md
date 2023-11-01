# Image Captioning

In this project, I aim to perform image captioning using convolutional and recurrent neural networks and obtain a textual description of an image from the model. Initially, I will attempt a simple approach by using **ResNet50** to convert the image into a rich feature vector and an **LSTM** network to generate text. In the first section, the ResNet50 network is used, and it **is frozen (except for the last layer, which is a linear layer that needs to be trained)**. In the second section of the project, I will add attention to this network and make some modifications to the network. The Flickr8k dataset is used for training the models, which consists of **8,000** images, each with **5 captions**. In the first section, only the tokens from the training data are used to create the vocabulary. However, in the second section, where attention is used, the tokens include all the tokens from the dataset, which are used in creating the vocabulary.

# Dependencies:
**Version of libraries:**
* **numpy : 1.23.5**
* **torch : 2.1.0+cu118**
* **torchtext : 0.16.0+cpu**
* **torchvision : 0.16.0+cu118**
* **tqdm : 4.66.1**
