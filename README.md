# CIAGAN: Conditional Identity Anonymization Generative Adversarial Networks
 
Official PyTorch implementation of [CIAGAN Conditional Identity Anonymization Generative Adversarial Networks](http://openaccess.thecvf.com/content_CVPR_2020/papers/Maximov_CIAGAN_Conditional_Identity_Anonymization_Generative_Adversarial_Networks_CVPR_2020_paper.pdf) published at Conference on Computer Vision and Pattern Recognition (CVPR) 2020.

## Installation

Please download the code:

To use our code, first download the repository:
````
git clone https://github.com/dvl-tum/ciagan.git
````

To install the dependencies:

````
pip install -r requirements.txt
````

## Training

In order to train a CIAGAN model, run the following command:

````
python run_training.py
````

We provided an example of our dataset that contains 5 identity folders from celebA dataset in the dataset folder. To train with full celebA dataset (or your own dataset), please setup the data in the same format. For the results generated in our paper, we trained the network using 1200 identities (each of them having at least 30 images) from celebA dataset. The identities can be found in: 

````
dataset/celeba/legit_indices.npy
````

## Citation

If you find this code useful, please consider citing the following paper:

````
@InProceedings{Maximov_2020_CVPR,
author = {Maximov, Maxim and Elezi, Ismail and Leal-Taixe, Laura},
title = {CIAGAN: Conditional Identity Anonymization Generative Adversarial Networks},
booktitle = {IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
month = {June},
year = {2020}
}
````
