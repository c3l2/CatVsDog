# CatVsDog
A classification model for recognizing cat and dog in a competition on DataCastle. Ranked 3/391. Utilized "Deep Residual Network" (original version). 

There are 4700 dog images but no cat images in the competition training data, so I picked totally 6501 cat images from ImageNet dataset, from subset n02123045, n02123159, n02123394, n02123597, and n02124075.

I trained the model applying a 50 layers Deep Residual Network model on Caffe. 

Following the common training setup, images are cropped to 224*224, and batch size is set to 16, and flipping is used for data augment, and weights are initialized with the pretrained ImageNet 1000-class classification model.

Note: The model I applied is the original Deep Residual Network from Kaiming He etc.'s CVPR2016 BEST paper "Deep residual learning for image recognition"(http://arxiv.org/abs/1512.03385). They further improve "Deep Residual Network" with pre-activation Residual Unit in paper "Identity Mappings in Deep Residual Networks"(http://arxiv.org/abs/1603.05027). 

Note: The training data is picked rather arbitrarily and params are not carefully tuned.
