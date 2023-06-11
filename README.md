# Self Supervised Learning for Fine grained Image Classification

As part of our project we have worked on using self supervised learning for fine grained classification of cassava leaves diseases. We've explored 3 different methods for applying self supervised learning - 
- [SRGAN](https://github.com/rush2406/Self-Supervised-Learning-for-Fine-grained-Image-Classification/tree/master/SRGAN)
- [Jigsaw as pretext task](https://github.com/rush2406/Self-Supervised-Learning-for-Fine-grained-Image-Classification/tree/master/Jigsaw_as_Pretext_task)
- [SimCLR](https://github.com/rush2406/Self-Supervised-Learning-for-Fine-grained-Image-Classification/tree/master/SimCLR)

The features learnt during the pretext task are fine tuned for downstream classification. The code (implemented in Pytorch) is separated into these 3 folders.

Our Baseline is a supervised fine grained classification model [Fine-Grained Visual Classiﬁcation via Progressive Multi-Granularity Training of Jigsaw Patches](https://arxiv.org/abs/2003.03836).

Do give a read at the [paper](https://arxiv.org/abs/2107.13973) for more details and analysis!

## Dataset

We have used the cassava leaves fine grained diseases dataset from Kaggle. The dataset has ~12K unlabelled images (extraimages.zip) and ~6K labelled images (train.zip).
The dataset can be downloaded from [here](https://www.kaggle.com/c/cassava-disease/data) and [here](https://www.kaggle.com/c/cassava-leaf-disease-classification/data?select=train_images). It has 5 disease classes as shown in the following order - cbb,cbsd,cgm,cmd,healthy

<img src = "images/cbb.jpg" alt = "cbb" width ="100" /> &nbsp; <img src = "images/cbsd.jpg" alt = "cbsd" width ="100" /> &nbsp; <img src = "images/cgm.jpg" alt = "cgm" width ="100" /> &nbsp; <img src = "images/cmd.jpg" alt = "cmd" width ="100" /> &nbsp; <img src = "images/healthy.jpg" alt="healthy" height = "133" width ="100" />

For the pretext task training, we've used the extra images (unlabelled). For the downstream task training, we've used the train images (labelled).

## General dependencies
```
python >= 3.6
torch
PIL
torchvision : conda install -c pytorch torchvision 
Opencv : pip install python-opencv
numpy : pip install numpy
scikit-learn : pip install -U numpy scipy scikit-learn
scipy : pip install scipy
```

## To run

We've included the code in the form of Jupyter notebooks to make it easy to visualize and run each cell. Further instructions have been provided in the README files of each folder.

## Credits

We are thankful to the authors of these projects for open sourcing their code

 [SRGAN](https://github.com/Lornatang/SRGAN-PyTorch) <br/>
 [Grad-CAM]( https://github.com/yaleCat/Grad-CAM-pytorch) <br/>
 [SimCLR](https://github.com/ssumin6/SimCLR) <br/>
 [Jigsaw pretext](https://github.com/aniket03/self_supervised_bird_classification) <br/>
 [PMG](https://github.com/PRIS-CV/PMG-Progressive-Multi-Granularity-Training)

## Citation

If you find this project useful, consider starring the repo and citing us in your work:

```
@misc{breiki2021selfsupervised,
      title={Self-Supervised Learning for Fine-Grained Image Classification}, 
      author={Farha Al Breiki and Muhammad Ridzuan and Rushali Grandhe},
      year={2021},
      eprint={2107.13973},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
