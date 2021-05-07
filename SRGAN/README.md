# Self Supervised Learning using SRGAN

[SRGAN](https://arxiv.org/abs/1609.04802) is a super-resolution generative adversarial network that creates high resolution images. The network downscales the images by a factor of four using a bicubic kernel and regenerates the images at two, four, and eight times the resolution. <br/>

We've experimented to understand the potential of the generator and discriminator of the model as a feature extractor using superresolution as pretext task. The features learnt to used fine tuned for downstream classification task.

## Instructions

The pretext task has been performed on the [extraimages](https://www.kaggle.com/c/cassava-disease/data?select=extraimages.zip) using the  instructions specified in this [repo](https://github.com/Lornatang/SRGAN-PyTorch). <br/>
The downstream classification task and modifications have been performed in the respective jupyter notebooks on the [train images](https://www.kaggle.com/c/cassava-disease/data?select=train.zip).<br/>

The jupyter can be run by each cell.

## To install

pip install torch-summary
pip install grad-cam

## Files

- images.txt - contains the image file names
- image_class_labels.txt - contains image to class mapping
- train_test_split.txt - contains split for train and validation
- SRGAN_discriminator.ipynb - contains code for using discriminator to perform downstream classification with different modifications such as changing input image sizes, different depths of ResNet backbone and added dropout. Code for visualizing Grad-CAM is also provided.
- SRGAN_generator.ipynb - contains code for using generator to perform downstream classification with different modifications such as changing input image sizes, different depths of ResNet backbone and added dropout.  Code for visualizing Grad-CAM is also provided.

## Credit

[SRGAN](https://github.com/Lornatang/SRGAN-PyTorch) <br/>
[Grad-CAM](https://github.com/yaleCat/Grad-CAM-pytorch)
