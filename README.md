# Neural Style Transfer

Implementation of neural style transfer from ["Image Style Transfer Using Convolutional Neural Networks" (Gatys et al., CVPR 2015).](https://openaccess.thecvf.com/content_cvpr_2016/papers/Gatys_Image_Style_Transfer_CVPR_2016_paper.pdf)

The general idea is to take two images, and produce a new image that reflects the content of one but the artistic "style" of the other. This is done through formulating a loss function that matches the content and style of each respective image in the feature space of a deep network, and then performing gradient descent on the pixels of the image itself.

The deep network used feature extractor is [SqueezeNet](https://arxiv.org/abs/1602.07360), a small model that has been trained on ImageNet, mainly for its small size and efficiency.

Additionally , this is extended to reconstruct an image from its feature representation - as shown in ["Understanding Deep Image Representations by Inverting them" (Mahendran et al., CVPR 2015)](https://arxiv.org/abs/1412.0035)
