# Automatic-Image-Captioning--Transfer-Learning - CNN/LSTM
Machine Learning Model- Uses Transfer Learning to generate Captions

*Also go through: "Requirements"- file thoroughly.*

DESCRIPTION OF REPOSITORY:

Dataset used: Flickr8k dataset

Flickr8k dataset is a dataset of photographs and descriptions. Flickr8k dataset comprises nearly 8091 photographs and their captions, with upto FIVE captions for each photograph. Since the dataset is large approximately 1 GB in size, I have attached a link to the dataset below here so that the original dataset can be downloaded and can be used into the model.

https://www.kaggle.com/adityajn105/flickr8k?select=Images

PACKAGES USED:
	1. Pandas, Tensorflow, Keras, Matplotlib, CV2, Numpy.


IMPLEMENTATION:

 I.The model uses is CNN-LSTM that makes use of Transfer Learning with InceptionV3 features, and GlovE embeddings. 

	-->InceptionV3 is a widely-used Image Recognition Model, evaluated on the ImageNet dataset.

	--> 200 dimensional GlovE embeddings have been used. 

 	--> *The extracted of Image features need to be dumped into a pickle file        * Pickle file is necessary due to cache memory issues.
  
  --> The Pickle files for the Image features are temporarory. The reason behind it is to keep this part as editable. The features can be varied according to the model.

II. TRAINING THE MODEL:

	--> The number of Epochs can be increased to improve the accuracy of the model.
	
	
Link to the GlovE embeddings: Please make use of 200dimensional embedding file. https://www.kaggle.com/datasets/anmolkumar/glove-embeddings


III. DEPLOYMENT OF THE MODEL:

	--> The running command to execute the deployment: python -m flask run
  	--> Deployed code is labelled as "Deployment Folder"
