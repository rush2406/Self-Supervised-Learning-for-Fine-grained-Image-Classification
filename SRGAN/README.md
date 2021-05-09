# Self-Supervised Learning Using SRGAN

[SRGAN](https://arxiv.org/abs/1609.04802) is a super-resolution generative adversarial network that upsamples low resolution images to create high resolution ones. The model is trained by downscaling an input image by a factor of four using a bicubic kernel and regenerating it at two, four, and eight times the resolution. <br/>

For our experiment, we separated the pre-trained generator and discriminator of the model to investigate the potential of each as a feature extractor using super-resolution as pretext task. The features learnt were transferred to the downstream classification task.

## To install

```pip install torch-summary``` <br/>
```pip install grad-cam```

## Instructions

The pretext task has been performed on the [extra images](https://www.kaggle.com/c/cassava-disease/data?select=extraimages.zip) using the instructions specified in this [repository](https://github.com/Lornatang/SRGAN-PyTorch). <br/>
The downstream classification task and modifications can be performed in their respective Jupyter notebooks (SRGAN_discriminator.ipynb and SRGAN_generator.ipynb) on the [train images](https://www.kaggle.com/c/cassava-disease/data?select=train.zip) from Kaggle.<br/>

## Files

- images.txt - contains the image file names
- image_class_labels.txt - contains image-to-class mapping
- train_test_split.txt - contains split for train and validation
- SRGAN_discriminator.ipynb - contains code for using discriminator to perform downstream classification with different modifications such as changing input image sizes, different depths of ResNet backbone and added dropout. Code for visualizing Grad-CAM is also provided.
- SRGAN_generator.ipynb - contains code for using generator to perform downstream classification with different modifications such as changing input image sizes, different depths of ResNet backbone and added dropout.  Code for visualizing Grad-CAM is also provided.
- demo folder - contains the demo code for SRGAN, where a class is predicted for a given input image (included with sample input and output)
 
## Credits

[SRGAN](https://github.com/Lornatang/SRGAN-PyTorch) - The base code for superresolution has been obtained from here. Downstream task and other modifications have been performed on top of this code <br/>
[Grad-CAM](https://github.com/yaleCat/Grad-CAM-pytorch) - The base code for Grad-CAM has been derived from here
