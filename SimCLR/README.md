# SimCLR

[SimCLR](https://arxiv.org/abs/2002.05709) is a self supervised learning algorithm based on contrastive loss, NT-Xent.

## Files

- SimCLR_Original.ipynb: Contains code for original SimCLR model with the default augmentations, except gaussain blur
- SimCLR_Gamma.ipynb: Contains modification for using Gamma transform and Grad-CAM visualization <br/>
  <img src = "../images/train-cgm-651.jpg" class="center" alt = "cbb" width ="50" /> &nbsp; <img src = "../images/gamma_image.jpg" class="center" alt = "gamma" width ="50" /> &nbsp;
- SimCLR_Cropped_regions.ipynb: Contains modifications for using Coarse Dropout and Grad-CAM visualization <br/>
  <img src = "../images/train-cgm-651.jpg" class="center" alt = "cbb" width ="50" /> &nbsp; <img src = "../images/dropout_image.jpg" class="center" alt = "gamma" width ="50" /> &nbsp;
- SimCLR_Random_swapping.ipynb: Contains modifications related to using random patch swap augmentation and Grad-CAM visualization <br/>
 <img src = "../images/train-cgm-651.jpg" class="center" alt = "cbb" width ="50" /> &nbsp; <img src = "../images/swapped.jpg" class="center" alt = "gamma" width ="50" /> &nbsp;
- SimCLR_Random_Jigsaw.ipynb: Contains modifications related to using random jigsaw augmentation and Grad-CAM visualization <br/>
  <img src = "../images/train-cgm-651.jpg" class="center" alt = "cbb" width ="50" /> &nbsp; <img src = "../images/random_jigsaw.jpg" class="center" alt = "gamma" height="65" width ="50" /> &nbsp;
- SimCLR_DCL_Jigsaw.ipynb: Contains modifications related to using [DCL](https://openaccess.thecvf.com/content_CVPR_2019/papers/Chen_Destruction_and_Construction_Learning_for_Fine-Grained_Image_Recognition_CVPR_2019_paper.pdf) based jigsaw shufflling <br/> augmentation and Grad-CAM visualization <br/>
  <img src = "../images/train-cgm-651.jpg" class="center" alt = "cbb" width ="50" /> &nbsp; <img src = "../images/dcl_jigsaw.jpg" class="center" alt = "gamma" width ="50" /> &nbsp;
- SimCLR_Cropped_regions.ipynb: Contains modifications related to localizing fine grained region [Smartcropping](https://github.com/fizzday/imageCropSmart) and Grad-CAM visualization <br/>
  <img src = "../images/train-cgm-651.jpg" class="center" alt = "cbb" width ="50" /> &nbsp; <img src = "../images/whiter.jpg" class="center" alt = "gamma" width ="50" /> &nbsp;
- Pretrained models folder: Contains saved models for each of the above augmentations
## To install

`pip install python-opencv` <br/>
`pip install -U albumentations` <br/>
`pip install git+https://github.com/fizzday/imageCropSmart` <br/>
  
## Credits
 
[SmartCrop](https://github.com/fizzday/imageCropSmart) <br/>
[Grad-CAM](https://github.com/yaleCat/Grad-CAM-pytorch) <br/>
[DCL](https://github.com/JDAI-CV/DCL) <br/>
[SimCLR](https://github.com/ssumin6/SimCLR)<br/>
