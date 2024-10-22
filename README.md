# Dog_Breed_Classification
Dog_Breed_Classification

## Overview
 "Dog_Breed_classification" is a competition focused on applying Deep Learning models to predict dog breeds from images. 
 
## Dataset
There are 70 unique breeds in total, with each image containing only one breed. You can find more information about the [competition](https://www.kaggle.com/competitions/dl-63-cw-image-classification).


## Details
The code for this competition was implemented using TensorFlow’s tensorflow.keras. The training dataset was split into a train-validation set with an 80-20 ratio. Data augmentation techniques were applied to both the training and validation sets, including:Rotation range, Width shift range, Height shift range, Shear range, Zoom range, Horizontal flip, Brightness range, Fill mode = 'nearest'.
I started with basic deep learning models like NNs and CNNs, but the results were unsatisfactory. To improve accuracy, I experimented with higher-level models such as EfficientNet, MobileNet, Inception, Xception, NasNet, .....

## Results 
The best performance was achieved by combining four models: InceptionResNetV2, InceptionV3, Xception, and NasNetLarge. 
This ensemble gave the highest accuracy with batch_size = 64 and target_size = 299 with the accuray on public test set is 0.97142 and private test set  is 0.97. When using a target_size of 331, the accuracy score on the public test set reached 0.96, while the highest accuracy on the private test set was 0.97285. 

Tuning hyperparameters had a significant impact on the results, demonstrating that in some cases, switching models can yield better outcomes.
