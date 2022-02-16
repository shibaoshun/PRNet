
# PRNet
## Convolution sparse coding with weighted L1 norm for Phase  retrieval : Algorithm and its deep unfoled network

## Abstract
Recovering the image of the interest from its phaseless measurment is the goal phase retrieval (PR). Recent PR algorithms that use hand-crafted priors suffer from low-quality reconstructions. To cope with this limitation, we exploit structural priors to propose a novel deep unfolded convolutional sparse coding phase retrieval network. Firstly, we formulate a weighted l1 norm (WL1) minimization problem utilizing convolutional sparse coding for PR, and solve it by using an iterative algorithm. An inertial epigraph method employing the inertial technique is proposed to solve the PR subproblem. Secondly, differing from updating weights of WL1 by using a fixed inverse proportional function in traditional methods, we learn such a function that can determine these crucial weights via a deep convolutional neural network equipped with the attention mechanism. Finally, we unroll the iterative PR algorithm to build a deep feedforward network architecture. Experiments demonstrate that the resulting model-based deep network can recover higherquality images, compared with the existing PR algorithms at various noise levels.

## Requirement
* Python 3.7.4
* PyTorch  1.7.0+cu110
* torchvision  0.4.1
* numpy 1.19.5

## How to obtain the trained models
You can download the trained models from any of the following paths:
* [https://pan.baidu.com/TrainedModels](https://pan.baidu.com/s/1hahrX4kiNiWKhEEGwZTqlQ),  and the extraction code of the file is `PRNN`.
* [https://1drv.ms/TrainedModels](https://1drv.ms/u/s!AssroyJstuZUgyeCCo0k2csKK7kB?e=Kgbojm)

## Testing
* The files of `PRNet_~dB` contain the trained models and the parameters of the ADAM optimizer at different noise levels.

* `Test_PRNet_SNR.py` is utilize to test the PSNR and SSIM values of the proposed PRNet on Set12.

* By modifying the the name of model and the value of SNR in `Test_PRNet_SNR.py`, evaluating the reconstruction quality of the proposed PRNet at different SNRs can be achieved.



