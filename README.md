# Dynamic-Neural-Network-Decoupling

PyTorch implementation for Dynamic Neural Network Decoupling.

## Running Code

In this code, you can run our Resnet-56 model on CIFAR10 dataset. The code has been tested by Python 3.5, [Pytorch 0.4.1](https://pytorch.org/) and CUDA 9.0 on Ubuntu 16.04.

## Running Example

### Train

#### CIFAR-10

##### ResNet-56

```shell
python train.py --net resnet56_architecture_decoupling \
                --pretrained True \
                --checkpoint pth/resnet56.pth \
                --train_dir tmp/resnet56_architecture_decoupling \
                --train_batch_size 128 \
                --learning_rate 0.01 \
                --epochs 200 \
                --schedule 100 \
                --Lambda_k 1 \
                --Lambda_m 0.005 \
                --Lambda_s 0.0001
```
