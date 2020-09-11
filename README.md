# Traffic-Signs-Classifer

Convolutional Neural network that identifies traffic signs using TensorFlow and OpenCV

This CNN classifies 50, 000+ images of different traffic signs. I am using OpenCV to process the images and then using a neural network created with TensorFlow for classification. Running this program with 15 epochs gives an accuracy of around ~95%. This neural net uses two convolutional layers (32 filters, 3x3 kernal), two max-pooling layers (2x2), and a hidden layer with 256 neurons with a 50% dropout rate. Below is some of my notes from my testing of this CNN.  

## 

• I'm getting good results using  32 filters using a 3x3 kernal, max pooling with a 2x2 layer and  a  hidden layer with 128 neutrons. Accuracy around ~85%

• By changing the max pooling size to a 4x4 grid, the accuracy went way down, to a final accuracy of 0.7468. I'm assuming the images are too small to use 4x4 pooling effectively

• using a convolution layer of 4x4 significantly increased the accuracy to 0.9579. Interestingly increasing  the hidden layers neurons to 248 with this  4x4 layer actually decreased accuracy slightly to 0.9341. Overfitting? 

• Now trying with two conv layers, both making 32 3x3 filters and two max pooling layers with a poolsize of 2x2, with a hidden layer of 256 neurons, gave me the best accuracy so far of 0.9596. The problem is this one was relatively slow, due to the hidden layer size.  
  
## 
[
<img width="932" alt="Screen Shot 2020-08-11 at 4 21 26 PM" src="https://user-images.githubusercontent.com/57844356/89955067-75e79780-dbef-11ea-95d1-e9b1df797f60.png">
](url)
##

*The dataset is from the German Traffic Sign Recognition Benchmark (gtsrb). http://benchmark.ini.rub.de/?section=gtsrb&subsection=news

