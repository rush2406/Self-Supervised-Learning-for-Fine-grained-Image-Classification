# SimCLR

[SimCLR](https://arxiv.org/abs/2002.05709) is a self supervised learning algorithm based on contrastive loss, NT-Xent.

## Files

- SimCLR_Original.ipynb: Contains code for original SimCLR model with the default augmentations, except gaussain blur
- SimCLR_Gamma.ipynb: Contains modification for using Gamma transform and Grad-CAM visualization
- SimCLR_Coarse_Dropout.ipynb: Contains modifications for using Coarse Dropout transform and Grad-CAM visualization
- SimCLR_Random_swapping.ipynb: Contains modifications related to using random patch swap augmentation and Grad-CAM visualization
- SimCLR_Random_Jigsaw.ipynb: Contains modifications related to using random jigsaw augmentation and Grad-CAM visualization
- SimCLR_DCL_Jigsaw.ipynb: Contains modifications related to using DCL based jigsaw shufflling augmentation and Grad-CAM visualization
- SimCLR_Cropped_regions.ipynb: Contains modifications related to  smartcropping of fine grained regions and Grad-CAM visualization 
