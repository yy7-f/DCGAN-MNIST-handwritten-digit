# DCGAN-MNIST-handwritten-digit
Developed DCGANs (Deep Convolutional Generative Adversarial Networks) with Pytorch to generate new data using MNIST handwritten digit data


Using GANs (Generative Adversarial Networks), you may create new data sets that closely resemble genuine data sets. 
However, GANs requires careful hyperparameter tunining in trainin process.
To solve the issue, DCGANs (Deep Convolutional Generative Adversarial Networks) is developed.   


DCGANs (Deep Convolutional Generative Adversarial Networks) mainly composes of convolution layers without max pooling or fully connected layers. It uses strided convolutions and transposed convolutions for the downsampling and the upsampling respectively.     

Architecture of stable DCGANs
• Replace all pooling layers with strided convolutions 
• Use batchnorm in both the generator and the discriminator.
• Remove fully connected hidden layers
• Use ReLU activation in generator for all layers except for the output (Tanh is used for the output)
• Use LeakyReLU activation in the discriminator for all layers.

<img width="581" alt="image" src="https://github.com/yy7-f/DCGAN-MNIST-handwritten-digit/assets/76237852/ac4aec20-bf4d-4a39-a85d-eeeb6caac62c">   

Results:

Generated data in the beginning of training:
<img width="374" alt="image" src="https://github.com/yy7-f/DCGAN-MNIST-handwritten-digit/assets/76237852/a217c0b5-23d7-4324-b241-e1d8534492ec">

Generated data in the end of training:
<img width="383" alt="image" src="https://github.com/yy7-f/DCGAN-MNIST-handwritten-digit/assets/76237852/f6d066f7-fef8-4cf8-b603-1bc8d1666346">


Reference:  
Radford, A., Metz, L., & Chintala, S. (2015). Unsupervised representation learning with deep convolutional generative adversarial networks. arXiv preprint arXiv:1511.06434.
