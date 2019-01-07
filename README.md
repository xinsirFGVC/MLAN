# MLAN

This is a PyTorch implementation of the paper "A multi-level attention network for fine-grained image classification" (Qi Xin, Tiejun Lv, and Hui Gao). We present the test code and a detailed code on CUB-200-2011 dataset for other researchers who interest in our work to reproduce our work.

## Requirements

The following are the experiment environment:
OS ubuntu 16.04
CUDA 9.0
CUDNN 7.0
Pytorch 0.4.1
4 NVIDIA 1080Ti GPU(at least 1 is required)
Note: please install jupyter to run the code provided.

## Datasets
You can download the three datasets from the official site:
for the bird dataset: 		http://www.vision.caltech.edu/visipedia/CUB-200-2011.html
for the car dataset:  		http://ai.stanford.edu/~jkrause/cars/car_dataset.html
for the aircraft dataset:	http://www.robots.ox.ac.uk/~vgg/data/fgvc-aircraft/
You should download the dataset and put it in the data folder. Then you should change the corresponding folder name in the code(You must do it or the code can't find the image) to fit the train.txt/test.txt in the data folder.

Note: In the data folder, we provide the train/test list for all of the three dataset.

## Visualize
We provide an extra code named bird_visulize to visualize the object/part localization on CUB-200-2011 method. We hope it can help you understand our method. You may need to extract the conv5_3 feature in order to visualize it. We provide you with some results that you can get directly when you open the file, if you don't want to reproduce it from scratch.

## Train the model
We provide a detailed code to train a MLAN on CUB-200-2011 dataset. You can just run the code we provided and you should get the same results. The training process is almost the same on Stanford-car and FGVC-Aircraft dataset, so you can reproduce it by yourself. If you have any question, please contact us. 

## Test the model
If you want to test the code, you should first download the dataset, and then download the models, then you should put them in the right folder, and you need to change the folder name in the code. Finally, Just run the jupyter notebook.

Note: There are some files named object_xx_xx.npy or part_xx_xx.npy, it is the object points and part points localized using our proposed method. You download it to test the model, and you can also generate it by yourself as we provide your the details in image_key_points_extraction.ipynb and feature_similarity_train.ipynb. 

## Model
We provide the trained model and associated files on https://pan.baidu.com/s/19333QinxHFV3E8TD8qVQfQ#list/path=%2FMLAN. You can download them directly or you can choose to train from scratch.
