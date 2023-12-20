# Neural_Network_project
In this repository, I present you my latest project related to Neural Networks - an algorithm which aims to recognize items on different images.

## Data Selection

The first dataset that has been chosen is created by Kritik Seth. He has gathered 36 different types of fruit and vegetables, each of which has approx. 100 examples and they are split into three folders/datasets with the following names and their distributions(%):

- train (80%)
- test (10%)
- validation (10%)

All of them will be used in this analysis to train the model well and later to validate its accuracy. Their metrics are saved in the Mlflow project run.

Then, the second dataset consists of images of fresh and stale fruit, from which only the images of the fresh ones will be trained on a new neural network. Since there are some inconsistencies in the classes between the two datasets, the following pre-processing will be done:

1. The second dataset contains only 6 classes of fruit and 12 folders (fresh/stale), they will be reduced to 5 classes of fresh fruit, as those are the fruit that can be found in the first dataset as well.
2. Then, the two datasets will be used together, by taking the train set of the first dataset as a validation set on the newly trained neural network. This will show how well the "fresh fruit" trained model classifies "fairly" new and different images of the same objects.

## References
1. The data used for training the original Neural Network has been obtained from Kaggle from the following source:
    Kritik Seth, "Fruits and Vegetables Image Recognition Dataset," Kaggle 2020 https://www.kaggle.com/kritikseth/fruit-and-vegetable-image-recognition

2. The validation data was taken from:
    Fresh and Stale Images of Fruits and Vegetables: https://www.kaggle.com/datasets/raghavrpotdar/fresh-and-stale-images-of-fruits-and-vegetables/data

