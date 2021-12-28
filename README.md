# cifar-restnet
Cifar classification using ResNet

Custom ResNet architecture for CIFAR10.

* Atleast two resnet blocks
* Initial conv block and final fully connected/Global avg pooling layer plus any number
of downscale/conv layers you might want to include
* 3x3 convolutions
* <5 million params

Use One Cycle Learning rate Policy and determine max learning rate to use.
Uses this transform -RandomCrop 32, 32 (after padding of 4),  FlipLR, Followed by CutOut(8, 8)
Target test accuracy 90%

Nice to have: use gradcam to find heatmaps for 10 incorrect labelled images.
Share code for augmentation, model definition, learning rate determination, and train/test logs.
