# Comparison of Modern Variants of Stochastic Gradient Descent (Application Mode)

#### The comparisions are given between Stochastic Gradient Descent (SGD), Heavy Ball(HB), Nesterov's Accelerated Gradient Descent (NAG), Accerlerated Stochastic Gradient Descent (ASGD) and Adam.

We provide the source code for our Term Paper for the Course EE609: Convex Optimization in Signal Processing and Communication. All the provided jupyter files can be run through Google Colab platform.

## Libraries Used
numpy
torch
torchvision
torchbearer
copy
matplotplib
tqdm
itertools
sklearn
random
scipy

Note: To install any of the above libraries:
1. Use "pip install *library_name*" for your local system.
2. Use "!pip install *library_name*" when installing on Colab

## Hardware used
GPU should be available at cuda:0

## Folder description
### Linear Regression
"*LinearRegression.ipynb*" performs Linear Regression on Discrete and Gaussiand Distributions with Stochastic Gradient Descent (SGD), Heavy Ball (HB), Nesterov's Accelerated Gradient Descent (NAG) and Accerlerated Stochastic Gradient Descent (ASGD), and outputs the relevant plots. One can also load the pre-saved loss values to reproduce the plots provided in out report.

"*GridSearchLinear.ipynb*" performs grid search for SGD, HB, NAG and ASGD and outputs the optimal hyperparameter values for Discrete and Gaussian Distributions.

### Deep Autoencoders
"*Autoencoders.ipynb*" conists of code for training the autoencoder on MNIST dataset and then plotting the result of performance comparision of various optimizers used on minibatch size 1 and 8.

"*Grid_Search.ipynb*" performs grid search on SGD, HB, NAG, ASGD and Adam to obtains the various parameters where they perform optimally. 

### Resnet
"*Resnet8.ipynb*" trains Resnet44 with Batch size 8 on CIFAR10 with SGD, HB, NAG, ASGD and Adam using a Decayed Hyperparameter Schedule. Their performances are compared using plots of suitable metrics. One can also load the pre-saved metrics to reproduce the plots provided in out report.

"*Resnet128.ipynb*" trains Resnet44 with Batch size 128 on CIFAR10 with SGD, HB, NAG, ASGD and Adam using both, a Decayed Hyperparameter Schedule and a Fixed Hyperparameter Schedule. Their performances are compared using plots of suitable metrics. One can also load the pre-saved metrics to reproduce the plots provided in out report.


## Possible Conflicts
1. https://github.com/HangZhongZH/Reproducible-report-of-On-the-insufficiency-of-existing-momentum-schemes-for-Stochastic-Optimization
2. https://github.com/COMP6248-Reproducability-Challenge/Insufficiency-momentum-schemes-for-Stochastic-Optimization

Note that most of the code base available on the above mentioned sources were hard coded to reproduce results similar to those declared in the original paper. We have cited urls in our code base, wherever we have imported code from other sources. (Such as code for ASGD optimizer, Resnet architecture, etc).


