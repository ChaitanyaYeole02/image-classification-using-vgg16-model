# VGG16 | CNN Model

<div align="justify">VGG is a convolutional neural network model proposed by K. Simonyan and A. Zisserman from the University of Oxford in the paper <a href="https://arxiv.org/abs/1409.1556" target="_top">“Very Deep Convolutional Networks for Large-Scale Image Recognition”</a>. It is a convolution neural net (CNN ) architecture which was used to win ILSVR(Imagenet) competition in 2014.</div>

<div align="justify">Most unique thing about VGG16 is that instead of having a large number of hyper-parameter they focused on having convolution layers of 3x3 filter with a stride 1 and always used same padding and maxpool layer of 2x2 filter of stride 2.</div> <br>

![vgg16 architecture](https://user-images.githubusercontent.com/35737777/69682136-5bdd4780-10a8-11ea-9079-50283f5451df.png) <br>

<div align="justify">It follows this arrangement of convolution and max pool layers consistently throughout the whole architecture. In the end it has 2 FC(fully connected layers) followed by a softmax for output. The 16 in VGG16 refers to it has 16 layers that have weights. This network is a pretty large network and it has about 138 million (approx) parameters.</div> <br>

![vgg16 layers](https://miro.medium.com/max/1400/1*UCGA58A2Ssjf74Z0Oh0_eQ.png)

### Convolution Layer
<div align="justify">A convolutional layer is the main building block of a CNN. It contains a set of filters (or kernels), parameters of which are to be learned throughout the training. The size of the filters is usually smaller than the actual image. Each filter convolves with the image and creates an activation map. For convolution the filter slid across the height and width of the image and the dot product between every element of the filter and the input is calculated at every spatial position.<br>Convolution is the first layer to extract features from an input image. It’s basically a mathematical operation that takes two inputs such as Image matrix and a filter or kernel. Convolution of an image with different filters can perform operations such as edge detection, blur and sharpen by applying filters.</div> <br>

![Alt Text](https://media.giphy.com/media/i4NjAwytgIRDW/giphy.gif)

### Pooling Layer
<div align="justify">A pooling layer is usually incorporated between two successive convolutional layers. The pooling layer reduces the number of parameters and computation by down-sampling the representation.

* Max Pooling – Largest element from the rectified feature map

* Average Pooling – Average of all the elements in the feature map

* Sum Pooling – Sum of all elements in the feature map 

</div> <br>

#### Limitations Of VGG 16:
<div align="justify">It is very slow to train (the original VGG model was trained on Nvidia Titan GPU for 2-3 weeks). The size of VGG-16 trained imageNet weights is 528 MB. So, it takes quite a lot of disk space and bandwidth which makes it inefficient.138 million parameters lead to exploding gradients problem.</div>
