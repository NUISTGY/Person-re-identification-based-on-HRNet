<h1 align="center"> Pytorch ReID </h1>
<h2 align="center"> Strong And Friendly </h2>
A re-ID baseline constructed by High-Resolution Network. With only a few necessary tricks, the rank-1 of Market-1501 is improved to 94.7%, which is much higher than the ResNet based method in the same dataset.
## Installation
- Install Pytorch from http://pytorch.org/
- Install Torchvision from the source
```
git clone https://github.com/pytorch/vision
cd vision
python setup.py install
```
- [Optinal] You may skip it. Install apex from the source
```
git clone https://github.com/NVIDIA/apex.git
cd apex
python setup.py install --cuda_ext --cpp_ext
```
Because pytorch and torchvision are ongoing projects.

Here we noted that our code is tested based on Pytorch 1.10.0 and CUDA 11.3 on Windows 11.

## Dataset & Preparation
Download [Market1501 Dataset](http://www.liangzheng.com.cn/Project/project_reid.html) [[Google]](https://drive.google.com/file/d/0B8-rUzbwVRk0c054eEozWG9COHM/view) [[Baidu]](https://pan.baidu.com/s/1ntIi2Op)

Preparation: Put the images with the same id in one folder. You may use 
```bash
python prepare.py
```
Remember to change the dataset path to your own path.

## Train & Test
Just following HRNet-reID.ipynb~
