# DCGAN with TF 2.0
  You need tensorflow 2.0 to run this code.


![mnist](https://user-images.githubusercontent.com/71681194/99708392-1d267580-2ae1-11eb-9073-9cb3ccc3afb1.JPG)

## Mode Collapse Problem
  At first I used MNIST with xavier initialization. As a result, mode collapse occured. Random normal initialization with std=0.02 solved the proplem. I think xavier made training faster so that overfitting occured. You can try reducing the number of epoch and using He normalization.


## Dataset
  I used LSUN church dataset which contain 126227 images. Shape of image is [64,64,3].

## Traning
  Training takes less than 1.5 hours with single rtx 2070 super. You should early stop the train when the results are good enough. It takes roughly 5 minutes for a epoch.

## Results
![result](https://user-images.githubusercontent.com/71681194/99709521-a25e5a00-2ae2-11eb-8e93-038b3af5c7eb.JPG)
