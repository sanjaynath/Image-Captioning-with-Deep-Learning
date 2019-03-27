# Image-Captioning-with-Deep-Learning
A deep learning model to generate descriptions for images. The model uses VGG for image encoding and LSTM network for text encoding and a Decoder to generate descriptions. 

The model has mainly 3 parts:

### Photo Feature Extractor. 
This is a 16-layer VGG model pre-trained on the ImageNet dataset. The photos are pre-processed with the VGG model (without the output layer) and the extracted features predicted by this model are used as input.
### Sequence Processor. 
This is a word embedding layer for handling the text input, followed by a Long Short-Term Memory (LSTM) recurrent neural network layer.
### Decoder
Both the feature extractor and sequence processor output a fixed-length vector. These are merged together and processed by a Dense layer to make a final prediction.
