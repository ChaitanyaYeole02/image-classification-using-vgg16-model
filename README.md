# Step by step VGG16 implementation in Keras

<div align="justify">VGG is a convolutional neural network model proposed by K. Simonyan and A. Zisserman from the University of Oxford in the paper [“Very Deep Convolutional Networks for Large-Scale Image Recognition”](https://arxiv.org/abs/1409.1556). It is a convolution neural net (CNN ) architecture which was used to win ILSVR(Imagenet) competition in 2014.</div>

\
Most unique thing about VGG16 is that instead of having a large number of hyper-parameter they focused on having convolution layers of 3x3 filter with a stride 1 and always used same padding and maxpool layer of 2x2 filter of stride 2.

![vgg16 architecture](https://user-images.githubusercontent.com/35737777/69682136-5bdd4780-10a8-11ea-9079-50283f5451df.png)

It follows this arrangement of convolution and max pool layers consistently throughout the whole architecture. In the end it has 2 FC(fully connected layers) followed by a softmax for output. The 16 in VGG16 refers to it has 16 layers that have weights. This network is a pretty large network and it has about 138 million (approx) parameters.

![vgg16 layers](https://miro.medium.com/max/1400/1*UCGA58A2Ssjf74Z0Oh0_eQ.png)
