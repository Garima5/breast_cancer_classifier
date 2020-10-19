# breast_cancer_classifier
Coded a Convolutional Neural Network using transfer learning to classify breast cancer images as benign or malignant. 
Used pretrained VGG 16 model and modified last layer. 
Added 2 fully connected layers in the end.

# Data Set
Used the breast cancer images provided in the BreakHis data set. It can be requested here: https://web.inf.ufpr.br/vri/databases/breast-cancer-histopathological-database-breakhis/

## Data Structure

### Original

### Rearranged the dataset as

# Libraries used
numpy
pandas
matplotlib
Opencv                
Keras 
Pytorch

# Important Observations

I trained the data for different learning rates and number of epochs. I observed that with learning rate = 0.02 and number of epochs = 25 I get about 85% test accuracy as well as decreasing error graph as:

If I train it for 30 epochs, I suspect the model overfits as the test error graph changes as:
!(0.05.png)
I learning rate is too low, say 0.001, the graph changes as:

