# Self Supervised Learning with Jigsaw as pretext task

In this method, we tried to use Jigsaw solving as a pretext task as explained in this [paper](https://arxiv.org/abs/1603.09246). The features learnt were then used for classification.


## Files

- images.txt - contains the image file names <br/>
- image_class_labels.txt - contains image to class mapping <br/>
- train_test_split.txt - contains split for train and validation <br/>
- Jigsaw_pretext.ipynb - contains code for using Jigsaw as pretext task and downstream classification <br/>

## To run

Download the [extraimages](https://www.kaggle.com/c/cassava-disease/data?select=extraimages.zip) and [train images](https://www.kaggle.com/c/cassava-disease/data?select=train.zip) <br/>
Then run the cells of the jupyter notebook 

## Credit

[Jigsaw as pretext task](https://github.com/aniket03/self_supervised_bird_classification/tree/500feb0d6f3cc95352ad94bd665499cfba0538b5) - The base code for Jigsaw solving as pretext task has been obtained from here
