# Self Supervised Learning using SRGAN

[SRGAN](https://arxiv.org/abs/1609.04802) is a super-resolution generative adversarial network that creates high resolution images. The network downscales the images by a factor of four using a bicubic kernel and regenerates the images at two, four, and eight times the resolution. <br/>

We've experimented to understand the potential of the generator and discriminator of the model as a feature extractor using superresolution as pretext task. The features learnt to used fine tuned for downstream classification task.

## Instructions to run/ Dependencies

(Add here if any)

## Files

- images.txt - contains the image file names
- image_class_labels.txt - contains image to class mapping
- train_test_split.txt - contains split for train and validation
- SRGAN_discriminator.ipynb - contains code for using discriminator to perform downstream classification (mention modifications here.....)
- SRGAN_generator.ipynb - contains code for using generator to perform downstream classification (mention modifications here.....)

## Credit

[SRGAN](https://github.com/Lornatang/SRGAN-PyTorch) <br/>
[Grad-CAM](https://github.com/yaleCat/Grad-CAM-pytorch)
