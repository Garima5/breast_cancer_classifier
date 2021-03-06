# Breast Cancer Classifier
* Coded a Convolutional Neural Network using transfer learning to classify breast cancer images as benign or malignant. 
* Used pretrained VGG 16 model and modified last layer. 
* Added 2 fully connected layers in the end.

# Data Set
Used the breast cancer images provided in the BreakHis data set. It can be requested here: https://web.inf.ufpr.br/vri/databases/breast-cancer-histopathological-database-breakhis/

## Data Structure

### Original
The original data folder looked like this 
![](images/ds1.png)
### Rearranged the dataset as
![](images/ds2.png)

# Libraries used
* numpy
* pandas
* matplotlib
* Opencv                
* Keras 
* Pytorch

# Important Observations

I trained the data for different learning rates and number of epochs. I observed that with learning rate = 0.02 and number of epochs = 25 I get about 85% test accuracy as well as decreasing error graph. If I train it for 30 epochs, the model supoosedely overfits as seen in the test error. For learning rate = 0.001, the error does decrease, however, the accuracy is about 73% only.

|  Learning Rate |  Number of Epochs |  Training error |  Testing error |
|----------------|---                |---|---|
| 0.02 |  25 | ![](images/0.02train.png) |  ![](images/0.02test.png) |
| 0.02  |  30 | ![](images/0.0230train.png)|![](images/0.0230test.png) |
| 0.001 |  25 | ![](images/0.001train.png)  | ![](images/0.001test.png)  |
| 0.01  |  25 | ![](images/0.01train.png)  | ![](images/0.01test.png)  |
| 0.05  |  25 | ![](images/0.05train.png)  | ![](images/0.05test.png) |
